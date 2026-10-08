# root

*Community 0 | 4 files | cohesion 1.00*

## Definition

This community groups 4 file(s) rooted at `root` with dominant language c (cohesion 1.00). Central symbols: `ACTION_LIST_FIRST`, `CALIB_LEN`, `CALIB_MARK_BYTE`, `CALIB_PATH`, `CALIB_PROBE_OFFSET`, `CALL_COUNT`, `FILTER_PRIO`, `IP_IHL_KEY_MASK`. Core file: `pedit_primitive.c` (55 symbols).

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `packet_edit_meme.c` | c | utility | 10 | no |
| `pedit_primitive.c` | c | utility | 55 | no |
| `pedit_primitive.h` | h | utility | 6 | no |
| `test_cve.c` | c | testing | 12 | no |

## Key Symbols

- `exec` (function, `packet_edit_meme.c:8`) `* and exec()s su, so the setuid bit makes it euid 0 globally and the corrupted *`
- `_GNU_SOURCE` (macro, `packet_edit_meme.c:20`) `#define _GNU_SOURCE`
- `SHELLCODE_PAD` (macro, `packet_edit_meme.c:33`) `#define SHELLCODE_PAD`
- `find_su` (function, `packet_edit_meme.c:58`) `static const char *find_su(void)`
- `elf_entry_offset` (function, `packet_edit_meme.c:72`) `static long elf_entry_offset(int fd)` - static const char *find_su(void) { struct stat info; int index; for (index = 0; SU_PATHS[index]; ind
- `write_proc_file` (function, `packet_edit_meme.c:94`) `static void write_proc_file(const char *path, const char *value)`
- `corrupt_entry` (function, `packet_edit_meme.c:108`) `static int corrupt_entry(int su_fd, long entry_offset)` - Runs in the unshare()d child: map to uid 0, then write the shellcode over su's * entry, slot by slot
- `run_exploit` (function, `packet_edit_meme.c:139`) `static int run_exploit(void)`
- `apparmor_userns_bypass` (function, `packet_edit_meme.c:212`) `static void apparmor_userns_bypass(char *self)`
- `main` (function, `packet_edit_meme.c:231`) `int main(int argc, char **argv)`
- `_GNU_SOURCE` (macro, `pedit_primitive.c:8`) `#define _GNU_SOURCE`
- `IP_IHL_KEY_OFFSET` (macro, `pedit_primitive.c:28`) `#define IP_IHL_KEY_OFFSET`
- `IP_IHL_KEY_VALUE` (macro, `pedit_primitive.c:29`) `#define IP_IHL_KEY_VALUE`
- `IP_IHL_KEY_MASK` (macro, `pedit_primitive.c:30`) `#define IP_IHL_KEY_MASK`
- `MAX_PEDIT_KEYS` (macro, `pedit_primitive.c:31`) `#define MAX_PEDIT_KEYS`
- `LOOPBACK_ADDR` (macro, `pedit_primitive.c:33`) `#define LOOPBACK_ADDR`
- `LOOPBACK_PREFIX` (macro, `pedit_primitive.c:34`) `#define LOOPBACK_PREFIX`
- `LOOPBACK_PORT` (macro, `pedit_primitive.c:35`) `#define LOOPBACK_PORT`
- `LISTEN_BACKLOG` (macro, `pedit_primitive.c:36`) `#define LISTEN_BACKLOG`
- `SETTLE_USEC` (macro, `pedit_primitive.c:37`) `#define SETTLE_USEC`
- `CALIB_PATH` (macro, `pedit_primitive.c:39`) `#define CALIB_PATH`
- `CALIB_LEN` (macro, `pedit_primitive.c:40`) `#define CALIB_LEN`
- `CALIB_PROBE_OFFSET` (macro, `pedit_primitive.c:41`) `#define CALIB_PROBE_OFFSET`
- `CALIB_MARK_BYTE` (macro, `pedit_primitive.c:42`) `#define CALIB_MARK_BYTE`
- `REQUEST_BUF_LEN` (macro, `pedit_primitive.c:44`) `#define REQUEST_BUF_LEN`
- `REPLY_BUF_LEN` (macro, `pedit_primitive.c:45`) `#define REPLY_BUF_LEN`
- `FILTER_PRIO` (macro, `pedit_primitive.c:46`) `#define FILTER_PRIO`
- `ACTION_LIST_FIRST` (macro, `pedit_primitive.c:47`) `#define ACTION_LIST_FIRST`
- `NLA_F_NESTED` (macro, `pedit_primitive.c:50`) `#define NLA_F_NESTED`
- `TC_H_CLSACT` (macro, `pedit_primitive.c:53`) `#define TC_H_CLSACT`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 3
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- No cross-community bridges recorded. This community is self-contained.

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- Why do 4 file(s) lack file-level docs (e.g. `packet_edit_meme.c`)? What purpose do they serve?
- What would break if the most connected file in root changed?
- Should root be split, given cohesion 1.00?

## Sources

- `packet_edit_meme.c`
- `pedit_primitive.c`
- `pedit_primitive.h`
- `test_cve.c`
