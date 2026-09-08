# Symbols

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `SHELLCODE_PAD` | macro | `packet_edit_meme.c:32` | `#define SHELLCODE_PAD` |
| `_GNU_SOURCE` | macro | `packet_edit_meme.c:20` | `#define _GNU_SOURCE` |
| `_exit` | function | `packet_edit_meme.c:185` | `_exit(0);` |
| `apparmor_userns_bypass` | function | `packet_edit_meme.c:211` | `static void apparmor_userns_bypass(char *self)` |
| `close` | function | `packet_edit_meme.c:102` | `close(fd);` |
| `corrupt_entry` | function | `packet_edit_meme.c:108` | `static int corrupt_entry(int su_fd, long entry_offset)` |
| `elf_entry_offset` | function | `packet_edit_meme.c:72` | `static long elf_entry_offset(int fd)` |
| `exec` | function | `packet_edit_meme.c:8` | `* and exec()s su, so the setuid bit makes it euid 0 globally and the corrupted * cached page runs the shellcode as real ` |
| `execlp` | function | `packet_edit_meme.c:223` | `execlp("aa-exec", "aa-exec", "-p", AA_PROFILES[index], "--", self, "--in-profile", (char *)NULL);` |
| `execve` | function | `packet_edit_meme.c:201` | `execve(su_path, su_argv, NULL);` |
| `find_su` | function | `packet_edit_meme.c:57` | `static const char *find_su(void)` |
| `fprintf` | function | `packet_edit_meme.c:152` | `fprintf(stderr, "[-] no setuid-root su found\n");` |
| `main` | function | `packet_edit_meme.c:230` | `int main(int argc, char **argv)` |
| `perror` | function | `packet_edit_meme.c:116` | `perror("unshare");` |
| `run_exploit` | function | `packet_edit_meme.c:138` | `static int run_exploit(void)` |
| `snprintf` | function | `packet_edit_meme.c:120` | `snprintf(map_line, sizeof(map_line), "0 %u 1", uid);` |
| `waitpid` | function | `packet_edit_meme.c:190` | `waitpid(child, &status, 0);` |
| `write_proc_file` | function | `packet_edit_meme.c:93` | `static void write_proc_file(const char *path, const char *value)` |
| `ACTION_LIST_FIRST` | macro | `pedit_primitive.c:47` | `#define ACTION_LIST_FIRST` |
| `CALIB_LEN` | macro | `pedit_primitive.c:40` | `#define CALIB_LEN` |
| `CALIB_MARK_BYTE` | macro | `pedit_primitive.c:42` | `#define CALIB_MARK_BYTE` |
| `CALIB_PATH` | macro | `pedit_primitive.c:38` | `#define CALIB_PATH` |
| `CALIB_PROBE_OFFSET` | macro | `pedit_primitive.c:41` | `#define CALIB_PROBE_OFFSET` |
| `FILTER_PRIO` | macro | `pedit_primitive.c:46` | `#define FILTER_PRIO` |
| `IP_IHL_KEY_MASK` | macro | `pedit_primitive.c:30` | `#define IP_IHL_KEY_MASK` |
| `IP_IHL_KEY_OFFSET` | macro | `pedit_primitive.c:27` | `#define IP_IHL_KEY_OFFSET` |
| `IP_IHL_KEY_VALUE` | macro | `pedit_primitive.c:29` | `#define IP_IHL_KEY_VALUE` |
| `LISTEN_BACKLOG` | macro | `pedit_primitive.c:36` | `#define LISTEN_BACKLOG` |
| `LOOPBACK_ADDR` | macro | `pedit_primitive.c:32` | `#define LOOPBACK_ADDR` |
| `LOOPBACK_PORT` | macro | `pedit_primitive.c:35` | `#define LOOPBACK_PORT` |
| `LOOPBACK_PREFIX` | macro | `pedit_primitive.c:34` | `#define LOOPBACK_PREFIX` |
| `MAX_PEDIT_KEYS` | macro | `pedit_primitive.c:31` | `#define MAX_PEDIT_KEYS` |
| `META_ID_PKTLEN` | macro | `pedit_primitive.c:74` | `#define META_ID_PKTLEN` |
| `META_ID_VALUE` | macro | `pedit_primitive.c:75` | `#define META_ID_VALUE` |
| `META_KIND_PKTLEN` | macro | `pedit_primitive.c:76` | `#define META_KIND_PKTLEN` |
| `META_KIND_VALUE` | macro | `pedit_primitive.c:77` | `#define META_KIND_VALUE` |
| `META_TYPE_INT` | macro | `pedit_primitive.c:73` | `#define META_TYPE_INT` |
| `MIN_DATA_PKT_LEN` | macro | `pedit_primitive.c:68` | `#define MIN_DATA_PKT_LEN` |
| `NLA_F_NESTED` | macro | `pedit_primitive.c:50` | `#define NLA_F_NESTED` |
| `REPLY_BUF_LEN` | macro | `pedit_primitive.c:45` | `#define REPLY_BUF_LEN` |
| `REQUEST_BUF_LEN` | macro | `pedit_primitive.c:43` | `#define REQUEST_BUF_LEN` |
| `SETTLE_USEC` | macro | `pedit_primitive.c:37` | `#define SETTLE_USEC` |
| `TCA_EM_META_HDR` | macro | `pedit_primitive.c:70` | `#define TCA_EM_META_HDR` |
| `TCA_EM_META_RVALUE` | macro | `pedit_primitive.c:71` | `#define TCA_EM_META_RVALUE` |
| `TCA_MATCHALL_ACT` | macro | `pedit_primitive.c:62` | `#define TCA_MATCHALL_ACT` |
| `TC_ACT_PIPE` | macro | `pedit_primitive.c:59` | `#define TC_ACT_PIPE` |
| `TC_H_CLSACT` | macro | `pedit_primitive.c:53` | `#define TC_H_CLSACT` |
| `TC_H_MIN_EGRESS` | macro | `pedit_primitive.c:56` | `#define TC_H_MIN_EGRESS` |
| `_GNU_SOURCE` | macro | `pedit_primitive.c:8` | `#define _GNU_SOURCE` |
| `api_fd_write` | function | `pedit_primitive.c:521` | `int api_fd_write(int fd, off_t offset, const void *src, size_t size)` |
| `append_pedit_action` | function | `pedit_primitive.c:295` | `static void append_pedit_action(const struct pedit_key_spec *keys, int key_count)` |
| `append_pktlen_ematch` | function | `pedit_primitive.c:258` | `static void append_pktlen_ematch(uint32_t threshold)` |
| `calibrate` | function | `pedit_primitive.c:437` | `static int calibrate(void)` |
| `close` | function | `pedit_primitive.c:407` | `close(client_fd);` |
| `clsact_add` | function | `pedit_primitive.c:239` | `static int clsact_add(int index)` |
| `clsact_delete` | function | `pedit_primitive.c:225` | `static void clsact_delete(int index)` |
| `egress_pedit_add` | function | `pedit_primitive.c:342` | `static int egress_pedit_add(int index, const struct pedit_key_spec *keys, int key_count)` |
| `ematch` | function | `pedit_primitive.c:339` | `* pkt_len ematch (only the data skb is touched, no out-of-range log spam);` |
| `fcntl` | function | `pedit_primitive.c:421` | `fcntl(client_fd, F_SETFL, O_NONBLOCK);` |
| `fill_ihl_key` | function | `pedit_primitive.c:373` | `static void fill_ihl_key(struct pedit_key_spec *key)` |
| `fsync` | function | `pedit_primitive.c:453` | `fsync(fd);` |
| `link_set_addr` | function | `pedit_primitive.c:499` | `link_set_addr(loopback_index, LOOPBACK_ADDR);` |
| `link_up` | function | `pedit_primitive.c:193` | `static int link_up(int index)` |
| `memcpy` | function | `pedit_primitive.c:129` | `memcpy(request_reserve(length), data, length);` |
| `memset` | function | `pedit_primitive.c:111` | `memset(request_buf, 0, sizeof(request_buf));` |
| `meta_header` | struct | `pedit_primitive.c:85` | `` |
| `meta_value` | struct | `pedit_primitive.c:79` | `` |
| `pedit_burst` | function | `pedit_primitive.c:384` | `static int pedit_burst(int src_fd, const struct pedit_key_spec *keys, int key_count)` |
| `pedit_key_spec` | struct | `pedit_primitive.c:90` | `` |
| `request_append` | function | `pedit_primitive.c:126` | `static void request_append(const void *data, int length)` |
| `request_attr` | function | `pedit_primitive.c:131` | `static void request_attr(int type, const void *data, int length)` |
| `request_attr_str` | function | `pedit_primitive.c:140` | `static void request_attr_str(int type, const char *text)` |
| `request_begin` | function | `pedit_primitive.c:108` | `static void request_begin(int type, int flags)` |
| `request_blob_begin` | function | `pedit_primitive.c:157` | `static struct rtattr *request_blob_begin(int type)` |
| `request_nest_begin` | function | `pedit_primitive.c:145` | `static struct rtattr *request_nest_begin(int type)` |
| `request_nest_end` | function | `pedit_primitive.c:165` | `static void request_nest_end(struct rtattr *attr)` |
| `request_reserve` | function | `pedit_primitive.c:118` | `static void *request_reserve(int length)` |
| `request_send` | function | `pedit_primitive.c:170` | `static int request_send(int allow_enoent)` |
| `setsockopt` | function | `pedit_primitive.c:504` | `setsockopt(listen_fd, SOL_SOCKET, SO_REUSEADDR, &reuse, sizeof(reuse));` |
| `setup` | function | `pedit_primitive.c:487` | `int setup(void)` |
| `unlink` | function | `pedit_primitive.c:479` | `unlink(CALIB_PATH);` |
| `usleep` | function | `pedit_primitive.c:427` | `usleep(SETTLE_USEC);` |
| `PEDIT_MAX_WRITE` | macro | `pedit_primitive.h:15` | `#define PEDIT_MAX_WRITE` |
| `PEDIT_PRIMITIVE_H` | macro | `pedit_primitive.h:9` | `#define PEDIT_PRIMITIVE_H` |
| `PEDIT_SLOT` | macro | `pedit_primitive.h:13` | `#define PEDIT_SLOT` |
| `api_fd_write` | function | `pedit_primitive.h:24` | `int api_fd_write(int fd, off_t offset, const void *src, size_t size);` |
| `bytes` | function | `pedit_primitive.h:3` | `* * Native write unit is 4 bytes (one pedit key == one u32 via skb_store_bits);` |
| `setup` | function | `pedit_primitive.h:19` | `int setup(void);` |
| `CALL_COUNT` | macro | `test_cve.c:19` | `#define CALL_COUNT` |
| `SRC_MIX_CALL` | macro | `test_cve.c:20` | `#define SRC_MIX_CALL` |
| `SRC_MIX_OFFSET` | macro | `test_cve.c:21` | `#define SRC_MIX_OFFSET` |
| `SRC_MIX_POS` | macro | `test_cve.c:22` | `#define SRC_MIX_POS` |
| `SRC_SEED` | macro | `test_cve.c:23` | `#define SRC_SEED` |
| `TARGET_LEN` | macro | `test_cve.c:18` | `#define TARGET_LEN` |
| `TARGET_PATH` | macro | `test_cve.c:16` | `#define TARGET_PATH` |
| `_GNU_SOURCE` | macro | `test_cve.c:9` | `#define _GNU_SOURCE` |
| `close` | function | `test_cve.c:58` | `close(fd);` |
| `create_target` | function | `test_cve.c:45` | `static int create_target(void)` |
| `fsync` | function | `test_cve.c:61` | `fsync(fd);` |
| `main` | function | `test_cve.c:65` | `int main(void)` |
| `make_source` | function | `test_cve.c:35` | `static void make_source(int call, off_t offset, uint8_t *src, size_t size)` |
| `printf` | function | `test_cve.c:75` | `printf("[-] create %s failed\n", TARGET_PATH);` |
| `write_case` | struct | `test_cve.c:25` | `` |
