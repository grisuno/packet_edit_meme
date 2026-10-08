# API

## packet_edit_meme.c

### find_su (function) `static const char *find_su(void)`
- Defined: `packet_edit_meme.c:58`
- Depends on: `pedit_primitive.h`

### elf_entry_offset (function) `static long elf_entry_offset(int fd)`
- Defined: `packet_edit_meme.c:72`
- Doc: static const char *find_su(void) { struct stat info; int index; for (index = 0; SU_PATHS[index]; index++) { if (stat(SU_
- Depends on: `pedit_primitive.h`

### write_proc_file (function) `static void write_proc_file(const char *path, const char *value)`
- Defined: `packet_edit_meme.c:94`
- Depends on: `pedit_primitive.h`

### corrupt_entry (function) `static int corrupt_entry(int su_fd, long entry_offset)`
- Defined: `packet_edit_meme.c:108`
- Doc: Runs in the unshare()d child: map to uid 0, then write the shellcode over su's * entry, slot by slot, through the page-c
- Depends on: `pedit_primitive.h`

### run_exploit (function) `static int run_exploit(void)`
- Defined: `packet_edit_meme.c:139`
- Depends on: `pedit_primitive.h`

### apparmor_userns_bypass (function) `static void apparmor_userns_bypass(char *self)`
- Defined: `packet_edit_meme.c:212`
- Depends on: `pedit_primitive.h`

### main (function) `int main(int argc, char **argv)`
- Defined: `packet_edit_meme.c:231`
- Depends on: `pedit_primitive.h`

### exec (function) `* and exec()s su, so the setuid bit makes it euid 0 globally and the corrupted * cached page runs the shellcode as real root. * * Shellcode is pure x86_64 syscalls (setuid=105, execve=59) -- the sysca`
- Defined: `packet_edit_meme.c:8`
- Depends on: `pedit_primitive.h`

## pedit_primitive.c

### request_begin (function) `static void request_begin(int type, int flags)`
- Defined: `pedit_primitive.c:109`
- Depends on: `pedit_primitive.h`

### request_reserve (function) `static void *request_reserve(int length)`
- Defined: `pedit_primitive.c:119`
- Depends on: `pedit_primitive.h`

### request_append (function) `static void request_append(const void *data, int length)`
- Defined: `pedit_primitive.c:127`
- Depends on: `pedit_primitive.h`

### request_attr (function) `static void request_attr(int type, const void *data, int length)`
- Defined: `pedit_primitive.c:132`
- Depends on: `pedit_primitive.h`

### request_attr_str (function) `static void request_attr_str(int type, const char *text)`
- Defined: `pedit_primitive.c:141`
- Depends on: `pedit_primitive.h`

### request_nest_begin (function) `static struct rtattr *request_nest_begin(int type)`
- Defined: `pedit_primitive.c:146`
- Depends on: `pedit_primitive.h`

### request_blob_begin (function) `static struct rtattr *request_blob_begin(int type)`
- Defined: `pedit_primitive.c:157`
- Doc: like request_nest_begin but without NLA_F_NESTED -- for the ematch entry whose * payload is a raw tcf_ematch_hdr followe
- Depends on: `pedit_primitive.h`

### request_nest_end (function) `static void request_nest_end(struct rtattr *attr)`
- Defined: `pedit_primitive.c:166`
- Depends on: `pedit_primitive.h`

### request_send (function) `static int request_send(int allow_enoent)`
- Defined: `pedit_primitive.c:171`
- Depends on: `pedit_primitive.h`

### link_up (function) `static int link_up(int index)`
- Defined: `pedit_primitive.c:194`
- Depends on: `pedit_primitive.h`

### clsact_delete (function) `static void clsact_delete(int index)`
- Defined: `pedit_primitive.c:226`
- Depends on: `pedit_primitive.h`

### clsact_add (function) `static int clsact_add(int index)`
- Defined: `pedit_primitive.c:240`
- Depends on: `pedit_primitive.h`

### append_pktlen_ematch (function) `static void append_pktlen_ematch(uint32_t threshold)`
- Defined: `pedit_primitive.c:258`
- Doc: request_begin(RTM_NEWQDISC, NLM_F_CREATE | NLM_F_EXCL); memset(&msg, 0, sizeof(msg)); msg.tcm_family = AF_UNSPEC; msg.tc
- Depends on: `pedit_primitive.h`

### append_pedit_action (function) `static void append_pedit_action(const struct pedit_key_spec *keys, int key_count)`
- Defined: `pedit_primitive.c:295`
- Doc: Emit one pedit action entry (kind + selector + per-key extensions) into the * action-list nest that the caller has alrea
- Depends on: `pedit_primitive.h`

### egress_pedit_add (function) `static int egress_pedit_add(int index, const struct pedit_key_spec *keys, int key_count)`
- Defined: `pedit_primitive.c:342`
- Doc: Install the egress pedit filter. Prefer the basic classifier scoped by a pkt_len ematch (only the data skb is touched, n
- Depends on: `pedit_primitive.h`

### fill_ihl_key (function) `static void fill_ihl_key(struct pedit_key_spec *key)`
- Defined: `pedit_primitive.c:374`
- Depends on: `pedit_primitive.h`

### pedit_burst (function) `static int pedit_burst(int src_fd, const struct pedit_key_spec *keys, int key_count)`
- Defined: `pedit_primitive.c:384`
- Doc: sendfile src_fd over a fresh loopback connection, arming `keys` on lo egress * only AFTER the handshake so the corruptio
- Depends on: `pedit_primitive.h`

### calibrate (function) `static int calibrate(void)`
- Defined: `pedit_primitive.c:437`
- Doc: Land a marker at a known key offset and read it back so api_fd_write() can * translate a file offset into the matching p
- Depends on: `pedit_primitive.h`

### setup (function) `int setup(void)`
- Defined: `pedit_primitive.c:488`
- Depends on: `pedit_primitive.h`

### api_fd_write (function) `int api_fd_write(int fd, off_t offset, const void *src, size_t size)`
- Defined: `pedit_primitive.c:522`
- Depends on: `pedit_primitive.h`

### ematch (function) `* pkt_len ematch (only the data skb is touched, no out-of-range log spam);`
- Defined: `pedit_primitive.c:339`
- Depends on: `pedit_primitive.h`

## pedit_primitive.h

### bytes (function) `* * Native write unit is 4 bytes (one pedit key == one u32 via skb_store_bits);`
- Defined: `pedit_primitive.h:4`
- Imported by: `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c`

### setup (function) `int setup(void);`
- Defined: `pedit_primitive.h:19`
- Doc: Bring lo up, open the loopback listener, calibrate the skb->file offset * delta. Returns 0 on success, -1 on failure.
- Imported by: `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c`

### api_fd_write (function) `int api_fd_write(int fd, off_t offset, const void *src, size_t size);`
- Defined: `pedit_primitive.h:24`
- Doc: Overwrite [offset, offset+size) of fd's page cache with src. fd may be O_RDONLY. size must be a multiple of PEDIT_SLOT a
- Imported by: `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c`

## test_cve.c

### make_source (function) `static void make_source(int call, off_t offset, uint8_t *src, size_t size)`
- Defined: `test_cve.c:36`
- Depends on: `pedit_primitive.h`

### create_target (function) `static int create_target(void)`
- Defined: `test_cve.c:46`
- Depends on: `pedit_primitive.h`

### main (function) `int main(void)`
- Defined: `test_cve.c:66`
- Depends on: `pedit_primitive.h`
