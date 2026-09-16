# Polyglot Codebase Knowledge Graph

> Generated offline by **readmenator**. 4 files, 103 symbols, 37 imports. Supports C, C++, Python, Go, Rust, JS/TS, Java, C#, Shell, PHP, Dart, GDScript, Nim, ASM, Ruby, Swift, Kotlin, Scala, Lua, Elixir.
> No LLMs. No tokens. Pure static analysis. See more [here](https://github.com/grisuno/ReadMenator)

**Start here:** Statistics Dashboard for scope, God Nodes for blast radius, Architecture Reference for per-file API. Agents: prefer `readmenator-agent/INDEX.md` + `SYMBOLS.md`.

**Total Files Parsed:** 4 | **Total Symbols Extracted:** 103 | **Total Imports:** 37
 | **Resolved Imports:** 3

<!-- ranking_model: v1.0 | weights: {ppr:0.45,auth:0.2,test:0.15,doc:0.1,fresh:0.1} | alpha:0.85 | commit:b3ca3bb | date:2026-07-18 -->


## Table of Contents

1. [Statistics Dashboard](#statistics-dashboard)
2. [Architectural Layers](#architectural-layers)
3. [Ranked Context](#ranked-context)
4. [God Nodes](#god-nodes)
5. [Community Analysis](#community-analysis)
6. [Suggested Questions](#suggested-questions)
7. [Hotspot Analysis](#hotspot-analysis)
8. [Change Impact Analysis](#change-impact-analysis)
9. [Suggested Linting Rules](#suggested-linting-rules)
10. [Orphans](#orphans)
11. [Query Recipes](#query-recipes)
12. [Structural Knowledge Map](#structural-knowledge-map)
13. [UML Class Diagram](#uml-class-diagram)
14. [Code Property Graph](#code-property-graph)
15. [Architecture Reference](#architecture-reference)
    - [C (3 files)](#c-3-files)
    - [H (1 files)](#h-1-files)

---

## Statistics Dashboard

| Metric | Value |
|--------|-------|
| Total Files | 4 |
| Total Symbols | 103 |
| Total Imports | 37 |
| Call Edges | 0 |
| Inheritance Edges | 0 |
| Languages | 2 |
| Avg Symbols/File | 25.8 |
| Avg Imports/File | 9.2 |
| Resolved Imports | 3 |

### Top Files by Import Count (Fan-Out)

| File | Imports | Symbols | Language |
|------|---------|---------|----------|
| `pedit_primitive.c` | 18 | 64 | c |
| `packet_edit_meme.c` | 11 | 18 | c |
| `test_cve.c` | 6 | 15 | c |
| `pedit_primitive.h` | 2 | 6 | h |

### Top Files by Imported-By Count (Fan-In)

| File | Imported By | Symbols | Language |
|------|-------------|---------|----------|
| `pedit_primitive.h` | 3 | 6 | h |

---

## Architectural Layers

Auto-detected from path patterns, naming conventions, and imported frameworks.

| Layer | Files |
|-------|-------|
| infrastructure | 3 |
| testing | 1 |

### infrastructure

- `packet_edit_meme.c` (c, 18 symbols)
- `pedit_primitive.c` (c, 64 symbols)
- `pedit_primitive.h` (h, 6 symbols)

### testing

- `test_cve.c` (c, 15 symbols)

---

## Ranked Context

Files ranked by composite score for the current query context. The ranking combines Personalized PageRank (query relevance), global authority, test coverage, documentation coverage, and code freshness. Model: v1.0.

| Rank | File | Composite | PPR | Authority | Test | Doc |
|------|------|-----------|-----|-----------|------|-----|
| 1 | `pedit_primitive.h` | 0.3856 | 0.5420 | 0.5420 | 0.00 | 0.33 |
| 2 | `pedit_primitive.c` | 0.1133 | 0.1527 | 0.1527 | 0.00 | 0.14 |
| 3 | `packet_edit_meme.c` | 0.1103 | 0.1527 | 0.1527 | 0.00 | 0.11 |
| 4 | `test_cve.c` | 0.0992 | 0.1527 | 0.1527 | 0.00 | 0.00 |

---

## God Nodes

Most architecturally central files ranked by combined import/export degree and symbol richness.

| File | Score | Connections | PageRank |
|------|-------|-------------|----------|
| `pedit_primitive.c` | 8.4 | | 0.1527 |
| `pedit_primitive.h` | 6.6 | | 0.5420 |
| `packet_edit_meme.c` | 3.8 | | 0.1527 |
| `test_cve.c` | 3.5 | | 0.1527 |

---

## Community Analysis

Files grouped by import-based community detection. Cohesion measures how tightly connected each community is internally.

### root (Cohesion: 1.00)

**4 files** in this community:

- `packet_edit_meme.c` (c, 18 symbols)
- `pedit_primitive.c` (c, 64 symbols)
- `pedit_primitive.h` (h, 6 symbols)
- `test_cve.c` (c, 15 symbols)

---

## Suggested Questions

Auto-generated exploration prompts based on graph structure:

- What does pedit_primitive.c depend on, and what depends on it? (1 connections)
- What does pedit_primitive.h depend on, and what depends on it? (3 connections)
- What does packet_edit_meme.c depend on, and what depends on it? (1 connections)
- How are the 4 files in 'root' related to each other?
- What is meta_value in pedit_primitive.c and how is it used?

---

## Hotspot Analysis

Files ranked by combined complexity (symbol count) and centrality (connection count). High-scoring files are architecturally critical and may need refactoring attention.

| File | Complexity | Centrality | Combined | Symbols | Connections |
|------|-----------|------------|----------|---------|-------------|
| `pedit_primitive.h` | 0.094 | 0.421 | 0.290 | 6 | 8 |
| `pedit_primitive.c` | 1.000 | 1.000 | 1.000 | 64 | 19 |
| `packet_edit_meme.c` | 0.281 | 0.632 | 0.491 | 18 | 12 |
| `test_cve.c` | 0.234 | 0.368 | 0.315 | 15 | 7 |

---

## Change Impact Analysis

Files sorted by how many other files would be affected if they changed. High-impact files should be changed with caution.

| File | Direct Dependents | Transitive Dependents | Total Impact |
|------|------------------|----------------------|--------------|
| `pedit_primitive.h` | 3 | 0 | 3 |
| `packet_edit_meme.c` | 0 | 0 | 0 |
| `pedit_primitive.c` | 0 | 0 | 0 |
| `test_cve.c` | 0 | 0 | 0 |

---

## Suggested Linting Rules

Automatically suggested linting and security rules based on patterns detected in the codebase. These can be exported as Semgrep rules using the `--export-rules` flag.

| Rule ID | Severity | Description | Language | Matches |
|---------|----------|-------------|----------|---------|
| `RM001` | info | Large number of functions in c: 52 total | c | 52 |
| `RM002` | info | Large number of functions in h: 3 total | h | 3 |

---

## Orphans

Files with no documentation or low connectivity. These are candidates for documentation investment or cleanup.

- `test_cve.c` (15 symbols, no doc)

---

## Query Recipes

Example queries you can run against this knowledge base using the ranking engine:

```
# Find files most relevant to a concept
readmenator query "Where is the import resolver implemented?"

# Rank files by relevance to a topic
readmenator query "How does documentation generation work?"

# Explain why a file ranks highly
readmenator query "explain readmenator/_documentation.py"

# Trace dependency paths with ranked context
readmenator query "path from CLI to exporter"
```

The ranking model uses the following signals:

- **Personalized PageRank** (45% weight): query-specific relevance via seed propagation
- **Global Authority** (20% weight): structural importance via standard PageRank
- **Test Coverage** (15% weight): fraction of symbols referenced in test files
- **Doc Coverage** (10% weight): presence of docstrings and file-level docs
- **Freshness** (10% weight): recent modification activity

Results include score decomposition and justification paths for each ranked item.

---

## Structural Knowledge Map

```mermaid
graph TD
    classDef mod fill:#1e1e1e,stroke:#ff6666,stroke-width:2px,color:#fff;
    classDef cls fill:#2d2d2d,stroke:#4ec9b0,stroke-width:2px,color:#fff;
    classDef fn fill:#333,stroke:#dcdcaa,stroke-width:1px,color:#dcdcaa;
    classDef ext fill:#111,stroke:#666,stroke-dasharray:5 5,color:#aaa;
    subgraph community_0 ["root"]
    pedit_primitive_c["pedit_primitive.c (c)"]
    class pedit_primitive_c mod;
    pedit_primitive_c_meta_value["meta_value"]
    class pedit_primitive_c_meta_value cls;
    pedit_primitive_c --> pedit_primitive_c_meta_value
    pedit_primitive_c_meta_header["meta_header"]
    class pedit_primitive_c_meta_header cls;
    pedit_primitive_c --> pedit_primitive_c_meta_header
    pedit_primitive_c_pedit_key_spec["pedit_key_spec"]
    class pedit_primitive_c_pedit_key_spec cls;
    pedit_primitive_c --> pedit_primitive_c_pedit_key_spec
    pedit_primitive_c_request_begin["request_begin"]
    class pedit_primitive_c_request_begin fn;
    pedit_primitive_c --> pedit_primitive_c_request_begin
    pedit_primitive_c_request_reserve["request_reserve"]
    class pedit_primitive_c_request_reserve fn;
    pedit_primitive_c --> pedit_primitive_c_request_reserve
    packet_edit_meme_c["packet_edit_meme.c (c)"]
    class packet_edit_meme_c mod;
    test_cve_c["test_cve.c (c)"]
    class test_cve_c mod;
    pedit_primitive_h["pedit_primitive.h (h)"]
    class pedit_primitive_h mod;
    end
    packet_edit_meme_c -- resolved_imports --> pedit_primitive_h
    pedit_primitive_c -- resolved_imports --> pedit_primitive_h
    test_cve_c -- resolved_imports --> pedit_primitive_h
    ext_pedit_primitive_h["pedit_primitive.h"]
    class ext_pedit_primitive_h ext;
    packet_edit_meme_c -.->|imports| ext_pedit_primitive_h
    ext_stdio_h["stdio.h"]
    class ext_stdio_h ext;
    packet_edit_meme_c -.->|imports| ext_stdio_h
    ext_stdlib_h["stdlib.h"]
    class ext_stdlib_h ext;
    packet_edit_meme_c -.->|imports| ext_stdlib_h
    ext_string_h["string.h"]
    class ext_string_h ext;
    packet_edit_meme_c -.->|imports| ext_string_h
    ext_errno_h["errno.h"]
    class ext_errno_h ext;
    packet_edit_meme_c -.->|imports| ext_errno_h
    ext_unistd_h["unistd.h"]
    class ext_unistd_h ext;
    packet_edit_meme_c -.->|imports| ext_unistd_h
    ext_fcntl_h["fcntl.h"]
    class ext_fcntl_h ext;
    packet_edit_meme_c -.->|imports| ext_fcntl_h
    ext_sched_h["sched.h"]
    class ext_sched_h ext;
    packet_edit_meme_c -.->|imports| ext_sched_h
    ext_elf_h["elf.h"]
    class ext_elf_h ext;
    packet_edit_meme_c -.->|imports| ext_elf_h
    ext_sys_stat_h["stat.h"]
    class ext_sys_stat_h ext;
    packet_edit_meme_c -.->|imports| ext_sys_stat_h
    ext_sys_wait_h["wait.h"]
    class ext_sys_wait_h ext;
    packet_edit_meme_c -.->|imports| ext_sys_wait_h
    pedit_primitive_c -.->|imports| ext_pedit_primitive_h
    pedit_primitive_c -.->|imports| ext_stdio_h
    pedit_primitive_c -.->|imports| ext_stdlib_h
    pedit_primitive_c -.->|imports| ext_string_h
    pedit_primitive_c -.->|imports| ext_errno_h
    pedit_primitive_c -.->|imports| ext_unistd_h
    pedit_primitive_c -.->|imports| ext_fcntl_h
    ext_sys_socket_h["socket.h"]
    class ext_sys_socket_h ext;
    pedit_primitive_c -.->|imports| ext_sys_socket_h
    ext_sys_sendfile_h["sendfile.h"]
    class ext_sys_sendfile_h ext;
    pedit_primitive_c -.->|imports| ext_sys_sendfile_h
    pedit_primitive_c -.->|imports| ext_sys_stat_h
    ext_arpa_inet_h["inet.h"]
    class ext_arpa_inet_h ext;
    pedit_primitive_c -.->|imports| ext_arpa_inet_h
    ext_net_if_h["if.h"]
    class ext_net_if_h ext;
    pedit_primitive_c -.->|imports| ext_net_if_h
    ext_linux_netlink_h["netlink.h"]
    class ext_linux_netlink_h ext;
    pedit_primitive_c -.->|imports| ext_linux_netlink_h
    ext_linux_rtnetlink_h["rtnetlink.h"]
    class ext_linux_rtnetlink_h ext;
    pedit_primitive_c -.->|imports| ext_linux_rtnetlink_h
    ext_linux_pkt_sched_h["pkt_sched.h"]
    class ext_linux_pkt_sched_h ext;
    pedit_primitive_c -.->|imports| ext_linux_pkt_sched_h
    ext_linux_pkt_cls_h["pkt_cls.h"]
    class ext_linux_pkt_cls_h ext;
    pedit_primitive_c -.->|imports| ext_linux_pkt_cls_h
    ext_linux_if_ether_h["if_ether.h"]
    class ext_linux_if_ether_h ext;
    pedit_primitive_c -.->|imports| ext_linux_if_ether_h
    ext_linux_tc_act_tc_pedit_h["tc_pedit.h"]
    class ext_linux_tc_act_tc_pedit_h ext;
    pedit_primitive_c -.->|imports| ext_linux_tc_act_tc_pedit_h
    ext_stdint_h["stdint.h"]
    class ext_stdint_h ext;
    pedit_primitive_h -.->|imports| ext_stdint_h
    ext_sys_types_h["types.h"]
    class ext_sys_types_h ext;
    pedit_primitive_h -.->|imports| ext_sys_types_h
    test_cve_c -.->|imports| ext_pedit_primitive_h
    test_cve_c -.->|imports| ext_stdio_h
    test_cve_c -.->|imports| ext_string_h
    test_cve_c -.->|imports| ext_stdint_h
    test_cve_c -.->|imports| ext_unistd_h
    test_cve_c -.->|imports| ext_fcntl_h
```

---

## UML Class Diagram

Auto-generated Mermaid class diagram from parsed class-level symbols. Shows classes, structs, interfaces, traits, and their methods with inheritance and dependency relationships.

```mermaid
classDiagram
  class pedit_primitive_c_meta_value {
    <<struct>>
    +request_begin(int type, int flags)
    +request_reserve(int length)
    +request_append(const void *data, int length)
    +request_attr(int type, const void *data, int length)
    +request_attr_str(int type, const char *text)
    +request_nest_begin(int type)
    +request_blob_begin(int type)
    +request_nest_end(struct rtattr *attr)
    +request_send(int allow_enoent)
    +link_up(int index)
  }
  class pedit_primitive_c_meta_header {
    <<struct>>
    +request_begin(int type, int flags)
    +request_reserve(int length)
    +request_append(const void *data, int length)
    +request_attr(int type, const void *data, int length)
    +request_attr_str(int type, const char *text)
    +request_nest_begin(int type)
    +request_blob_begin(int type)
    +request_nest_end(struct rtattr *attr)
    +request_send(int allow_enoent)
    +link_up(int index)
  }
  class pedit_primitive_c_pedit_key_spec {
    <<struct>>
    +request_begin(int type, int flags)
    +request_reserve(int length)
    +request_append(const void *data, int length)
    +request_attr(int type, const void *data, int length)
    +request_attr_str(int type, const char *text)
    +request_nest_begin(int type)
    +request_blob_begin(int type)
    +request_nest_end(struct rtattr *attr)
    +request_send(int allow_enoent)
    +link_up(int index)
  }
  class test_cve_c_write_case {
    <<struct>>
    +make_source(int call, off_t offset, uint8_t *src, size_t size)
    +create_target(void)
    +main(void)
    +close(fd);
    +fsync(fd);
    +printf("[-] create %s failed\n", TARGET_PATH);
  }
```

---

## Code Property Graph

Machine-readable Code Property Graph (CPG) in JSON-LD format. This block allows AI agents to parse the full structural graph without additional file reads. Compatible with GraphRAG pipelines.

```json
{"@context": "https://schema.org", "analysis": {"communities": [{"cohesion": 1.0, "id": 0, "label": "root", "size": 4}], "god_nodes": [{"node_id": "pedit_primitive.c", "score": 8.4}, {"node_id": "pedit_primitive.h", "score": 6.6}, {"node_id": "packet_edit_meme.c", "score": 3.8}, {"node_id": "test_cve.c", "score": 3.5}], "surprising_connections": []}, "edges": [{"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "pedit_primitive.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "stdio.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "stdlib.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "string.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "errno.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "unistd.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "fcntl.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "sched.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "elf.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "sys/stat.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "packet_edit_meme.c", "target": "sys/wait.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "pedit_primitive.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "stdio.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "stdlib.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "string.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "errno.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "unistd.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "fcntl.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "sys/socket.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "sys/sendfile.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "sys/stat.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "arpa/inet.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "net/if.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "linux/netlink.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "linux/rtnetlink.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "linux/pkt_sched.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "linux/pkt_cls.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "linux/if_ether.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.c", "target": "linux/tc_act/tc_pedit.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.h", "target": "stdint.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "pedit_primitive.h", "target": "sys/types.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "test_cve.c", "target": "pedit_primitive.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "test_cve.c", "target": "stdio.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "test_cve.c", "target": "string.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "test_cve.c", "target": "stdint.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "test_cve.c", "target": "unistd.h"}, {"confidence": "EXTRACTED", "relation": "imports", "source": "test_cve.c", "target": "fcntl.h"}, {"confidence": "EXTRACTED", "relation": "resolved_imports", "source": "packet_edit_meme.c", "target": "pedit_primitive.h"}, {"confidence": "EXTRACTED", "relation": "resolved_imports", "source": "pedit_primitive.c", "target": "pedit_primitive.h"}, {"confidence": "EXTRACTED", "relation": "resolved_imports", "source": "test_cve.c", "target": "pedit_primitive.h"}], "generator": "readmenator", "metadata": {"edge_count": 40, "file_count": 4, "language_count": 2, "symbol_count": 103}, "nodes": [{"id": "packet_edit_meme.c", "kind": "module", "label": "packet_edit_meme.c", "language": "c", "sha256": "3641dfb8999b22f1", "symbol_count": 18, "symbols": [{"kind": "function", "line": 57, "name": "find_su", "signature": "static const char *find_su(void)"}, {"doc": "static const char *find_su(void) { struct stat info; int index; for (index = 0; SU_PATHS[index]; index++) { if (stat(SU_PATHS[index], &info) == 0 && S_ISREG(info.st_mode) && (info.st_mode & S_ISUID) && info.st_uid == 0) return SU_PATHS[index]; } return NULL; } /* Return the file offset of e_entry via the executable PT_LOAD that contains it.", "kind": "function", "line": 72, "name": "elf_entry_offset", "signature": "static long elf_entry_offset(int fd)"}, {"kind": "function", "line": 93, "name": "write_proc_file", "signature": "static void write_proc_file(const char *path, const char *value)"}, {"doc": "Runs in the unshare()d child: map to uid 0, then write the shellcode over su's * entry, slot by slot, through the page-cache primitive.", "kind": "function", "line": 108, "name": "corrupt_entry", "signature": "static int corrupt_entry(int su_fd, long entry_offset)"}, {"kind": "function", "line": 138, "name": "run_exploit", "signature": "static int run_exploit(void)"}, {"kind": "function", "line": 211, "name": "apparmor_userns_bypass", "signature": "static void apparmor_userns_bypass(char *self)"}, {"kind": "function", "line": 230, "name": "main", "signature": "int main(int argc, char **argv)"}, {"kind": "function", "line": 8, "name": "exec", "signature": "* and exec()s su, so the setuid bit makes it euid 0 globally and the corrupted * cached page runs the shellcode as real root. * * Shellcode is pure x86_64 syscalls (setuid=105, execve=59) -- the sysca"}, {"kind": "function", "line": 102, "name": "close", "signature": "close(fd);"}, {"kind": "function", "line": 116, "name": "perror", "signature": "perror(\"unshare\");"}, {"kind": "function", "line": 120, "name": "snprintf", "signature": "snprintf(map_line, sizeof(map_line), \"0 %u 1\", uid);"}, {"kind": "function", "line": 152, "name": "fprintf", "signature": "fprintf(stderr, \"[-] no setuid-root su found\\n\");"}, {"kind": "function", "line": 185, "name": "_exit", "signature": "_exit(0);"}, {"kind": "function", "line": 190, "name": "waitpid", "signature": "waitpid(child, &status, 0);"}, {"kind": "function", "line": 201, "name": "execve", "signature": "execve(su_path, su_argv, NULL);"}, {"kind": "function", "line": 223, "name": "execlp", "signature": "execlp(\"aa-exec\", \"aa-exec\", \"-p\", AA_PROFILES[index], \"--\", self, \"--in-profile\", (char *)NULL);"}, {"kind": "macro", "line": 20, "name": "_GNU_SOURCE", "signature": "#define _GNU_SOURCE"}, {"kind": "macro", "line": 32, "name": "SHELLCODE_PAD", "signature": "#define SHELLCODE_PAD"}]}, {"id": "pedit_primitive.c", "kind": "module", "label": "pedit_primitive.c", "language": "c", "sha256": "27251b9bb57a8b32", "symbol_count": 64, "symbols": [{"kind": "struct", "line": 79, "name": "meta_value"}, {"kind": "struct", "line": 85, "name": "meta_header"}, {"kind": "struct", "line": 90, "name": "pedit_key_spec"}, {"kind": "function", "line": 108, "name": "request_begin", "signature": "static void request_begin(int type, int flags)"}, {"kind": "function", "line": 118, "name": "request_reserve", "signature": "static void *request_reserve(int length)"}, {"kind": "function", "line": 126, "name": "request_append", "signature": "static void request_append(const void *data, int length)"}, {"kind": "function", "line": 131, "name": "request_attr", "signature": "static void request_attr(int type, const void *data, int length)"}, {"kind": "function", "line": 140, "name": "request_attr_str", "signature": "static void request_attr_str(int type, const char *text)"}, {"kind": "function", "line": 145, "name": "request_nest_begin", "signature": "static struct rtattr *request_nest_begin(int type)"}, {"doc": "like request_nest_begin but without NLA_F_NESTED -- for the ematch entry whose * payload is a raw tcf_ematch_hdr followed by attributes.", "kind": "function", "line": 157, "name": "request_blob_begin", "signature": "static struct rtattr *request_blob_begin(int type)"}, {"kind": "function", "line": 165, "name": "request_nest_end", "signature": "static void request_nest_end(struct rtattr *attr)"}, {"kind": "function", "line": 170, "name": "request_send", "signature": "static int request_send(int allow_enoent)"}, {"doc": "return -1; received = recv(netlink_fd, reply_buf, sizeof(reply_buf), 0); if (received < 0) return -1; reply = (struct nlmsghdr *)reply_buf; if (reply->nlmsg_type != NLMSG_ERROR) return 0; reply_error = NLMSG_DATA(reply); if (reply_error->error && !(allow_enoent && reply_error->error == -ENOENT)) return reply_error->error; return 0; } /* ============================== link / qdisc ==============================", "kind": "function", "line": 193, "name": "link_up", "signature": "static int link_up(int index)"}, {"kind": "function", "line": 225, "name": "clsact_delete", "signature": "static void clsact_delete(int index)"}, {"kind": "function", "line": 239, "name": "clsact_add", "signature": "static int clsact_add(int index)"}, {"doc": "request_begin(RTM_NEWQDISC, NLM_F_CREATE | NLM_F_EXCL); memset(&msg, 0, sizeof(msg)); msg.tcm_family = AF_UNSPEC; msg.tcm_ifindex = index; msg.tcm_handle = TC_H_MAKE(TC_H_CLSACT, 0); msg.tcm_parent = TC_H_CLSACT; request_append(&msg, sizeof(msg)); request_attr_str(TCA_KIND, \"clsact\"); return request_send(0); } /* ============================== pedit filter ============================== /* basic-classifier ematch tree that matches only skbs with skb->len > threshold.", "kind": "function", "line": 258, "name": "append_pktlen_ematch", "signature": "static void append_pktlen_ematch(uint32_t threshold)"}, {"doc": "Emit one pedit action entry (kind + selector + per-key extensions) into the * action-list nest that the caller has already opened.", "kind": "function", "line": 295, "name": "append_pedit_action", "signature": "static void append_pedit_action(const struct pedit_key_spec *keys, int key_count)"}, {"doc": "Install the egress pedit filter. Prefer the basic classifier scoped by a pkt_len ematch (only the data skb is touched, no out-of-range log spam); on kernels without cls_basic / em_meta (e.g. RHEL) fall back to matchall, which * fires on every egress skb -- still armed only after the handshake.", "kind": "function", "line": 342, "name": "egress_pedit_add", "signature": "static int egress_pedit_add(int index, const struct pedit_key_spec *keys, int key_count)"}, {"doc": "action_list = request_nest_begin(TCA_MATCHALL_ACT); } else { request_attr_str(TCA_KIND, \"basic\"); options = request_nest_begin(TCA_OPTIONS); append_pktlen_ematch(MIN_DATA_PKT_LEN); // match only the sendfile data skb action_list = request_nest_begin(TCA_BASIC_ACT); } append_pedit_action(keys, key_count); request_nest_end(action_list); request_nest_end(options); return request_send(0); } /* ============================== burst engine ==============================", "kind": "function", "line": 373, "name": "fill_ihl_key", "signature": "static void fill_ihl_key(struct pedit_key_spec *key)"}, {"doc": "sendfile src_fd over a fresh loopback connection, arming `keys` on lo egress * only AFTER the handshake so the corruption rides the data, not the SYNs.", "kind": "function", "line": 384, "name": "pedit_burst", "signature": "static int pedit_burst(int src_fd, const struct pedit_key_spec *keys, int key_count)"}, {"doc": "Land a marker at a known key offset and read it back so api_fd_write() can * translate a file offset into the matching pedit key offset on any geometry.", "kind": "function", "line": 437, "name": "calibrate", "signature": "static int calibrate(void)"}, {"doc": "buf[index_iter + 3] == CALIB_MARK_BYTE) { landed = index_iter; break; } } close(fd); unlink(CALIB_PATH); if (landed < 0) return -1; offset_delta = landed - CALIB_PROBE_OFFSET; return 0; } /* ================================= api ====================================", "kind": "function", "line": 487, "name": "setup", "signature": "int setup(void)"}, {"kind": "function", "line": 521, "name": "api_fd_write", "signature": "int api_fd_write(int fd, off_t offset, const void *src, size_t size)"}, {"kind": "function", "line": 111, "name": "memset", "signature": "memset(request_buf, 0, sizeof(request_buf));"}, {"kind": "function", "line": 129, "name": "memcpy", "signature": "memcpy(request_reserve(length), data, length);"}, {"kind": "function", "line": 339, "name": "ematch", "signature": "* pkt_len ematch (only the data skb is touched, no out-of-range log spam);"}, {"kind": "function", "line": 407, "name": "close", "signature": "close(client_fd);"}, {"kind": "function", "line": 421, "name": "fcntl", "signature": "fcntl(client_fd, F_SETFL, O_NONBLOCK);"}, {"kind": "function", "line": 427, "name": "usleep", "signature": "usleep(SETTLE_USEC);"}, {"kind": "function", "line": 453, "name": "fsync", "signature": "fsync(fd);"}, {"kind": "function", "line": 479, "name": "unlink", "signature": "unlink(CALIB_PATH);"}, {"kind": "function", "line": 499, "name": "link_set_addr", "signature": "link_set_addr(loopback_index, LOOPBACK_ADDR);"}, {"kind": "function", "line": 504, "name": "setsockopt", "signature": "setsockopt(listen_fd, SOL_SOCKET, SO_REUSEADDR, &reuse, sizeof(reuse));"}, {"kind": "macro", "line": 8, "name": "_GNU_SOURCE", "signature": "#define _GNU_SOURCE"}, {"kind": "macro", "line": 27, "name": "IP_IHL_KEY_OFFSET", "signature": "#define IP_IHL_KEY_OFFSET"}, {"kind": "macro", "line": 29, "name": "IP_IHL_KEY_VALUE", "signature": "#define IP_IHL_KEY_VALUE"}, {"kind": "macro", "line": 30, "name": "IP_IHL_KEY_MASK", "signature": "#define IP_IHL_KEY_MASK"}, {"kind": "macro", "line": 31, "name": "MAX_PEDIT_KEYS", "signature": "#define MAX_PEDIT_KEYS"}, {"kind": "macro", "line": 32, "name": "LOOPBACK_ADDR", "signature": "#define LOOPBACK_ADDR"}, {"kind": "macro", "line": 34, "name": "LOOPBACK_PREFIX", "signature": "#define LOOPBACK_PREFIX"}, {"kind": "macro", "line": 35, "name": "LOOPBACK_PORT", "signature": "#define LOOPBACK_PORT"}, {"kind": "macro", "line": 36, "name": "LISTEN_BACKLOG", "signature": "#define LISTEN_BACKLOG"}, {"kind": "macro", "line": 37, "name": "SETTLE_USEC", "signature": "#define SETTLE_USEC"}, {"kind": "macro", "line": 38, "name": "CALIB_PATH", "signature": "#define CALIB_PATH"}, {"kind": "macro", "line": 40, "name": "CALIB_LEN", "signature": "#define CALIB_LEN"}, {"kind": "macro", "line": 41, "name": "CALIB_PROBE_OFFSET", "signature": "#define CALIB_PROBE_OFFSET"}, {"kind": "macro", "line": 42, "name": "CALIB_MARK_BYTE", "signature": "#define CALIB_MARK_BYTE"}, {"kind": "macro", "line": 43, "name": "REQUEST_BUF_LEN", "signature": "#define REQUEST_BUF_LEN"}, {"kind": "macro", "line": 45, "name": "REPLY_BUF_LEN", "signature": "#define REPLY_BUF_LEN"}, {"kind": "macro", "line": 46, "name": "FILTER_PRIO", "signature": "#define FILTER_PRIO"}, {"kind": "macro", "line": 47, "name": "ACTION_LIST_FIRST", "signature": "#define ACTION_LIST_FIRST"}, {"kind": "macro", "line": 50, "name": "NLA_F_NESTED", "signature": "#define NLA_F_NESTED"}, {"kind": "macro", "line": 53, "name": "TC_H_CLSACT", "signature": "#define TC_H_CLSACT"}, {"kind": "macro", "line": 56, "name": "TC_H_MIN_EGRESS", "signature": "#define TC_H_MIN_EGRESS"}, {"kind": "macro", "line": 59, "name": "TC_ACT_PIPE", "signature": "#define TC_ACT_PIPE"}, {"kind": "macro", "line": 62, "name": "TCA_MATCHALL_ACT", "signature": "#define TCA_MATCHALL_ACT"}, {"kind": "macro", "line": 68, "name": "MIN_DATA_PKT_LEN", "signature": "#define MIN_DATA_PKT_LEN"}, {"kind": "macro", "line": 70, "name": "TCA_EM_META_HDR", "signature": "#define TCA_EM_META_HDR"}, {"kind": "macro", "line": 71, "name": "TCA_EM_META_RVALUE", "signature": "#define TCA_EM_META_RVALUE"}, {"kind": "macro", "line": 73, "name": "META_TYPE_INT", "signature": "#define META_TYPE_INT"}, {"kind": "macro", "line": 74, "name": "META_ID_PKTLEN", "signature": "#define META_ID_PKTLEN"}, {"kind": "macro", "line": 75, "name": "META_ID_VALUE", "signature": "#define META_ID_VALUE"}, {"kind": "macro", "line": 76, "name": "META_KIND_PKTLEN", "signature": "#define META_KIND_PKTLEN"}, {"kind": "macro", "line": 77, "name": "META_KIND_VALUE", "signature": "#define META_KIND_VALUE"}]}, {"id": "pedit_primitive.h", "kind": "module", "label": "pedit_primitive.h", "language": "h", "sha256": "024424d8711c7ec7", "symbol_count": 6, "symbols": [{"kind": "function", "line": 3, "name": "bytes", "signature": "* * Native write unit is 4 bytes (one pedit key == one u32 via skb_store_bits);"}, {"doc": "Bring lo up, open the loopback listener, calibrate the skb->file offset * delta. Returns 0 on success, -1 on failure.", "kind": "function", "line": 19, "name": "setup", "signature": "int setup(void);"}, {"doc": "Overwrite [offset, offset+size) of fd's page cache with src. fd may be O_RDONLY. size must be a multiple of PEDIT_SLOT and <= PEDIT_MAX_WRITE, else * the call is refused. Idempotent. Returns 0 on success, -1 otherwise.", "kind": "function", "line": 24, "name": "api_fd_write", "signature": "int api_fd_write(int fd, off_t offset, const void *src, size_t size);"}, {"kind": "macro", "line": 9, "name": "PEDIT_PRIMITIVE_H", "signature": "#define PEDIT_PRIMITIVE_H"}, {"kind": "macro", "line": 13, "name": "PEDIT_SLOT", "signature": "#define PEDIT_SLOT"}, {"kind": "macro", "line": 15, "name": "PEDIT_MAX_WRITE", "signature": "#define PEDIT_MAX_WRITE"}]}, {"id": "test_cve.c", "kind": "module", "label": "test_cve.c", "language": "c", "sha256": "8446e9053cd0cd70", "symbol_count": 15, "symbols": [{"kind": "struct", "line": 25, "name": "write_case"}, {"kind": "function", "line": 35, "name": "make_source", "signature": "static void make_source(int call, off_t offset, uint8_t *src, size_t size)"}, {"kind": "function", "line": 45, "name": "create_target", "signature": "static int create_target(void)"}, {"kind": "function", "line": 65, "name": "main", "signature": "int main(void)"}, {"kind": "function", "line": 58, "name": "close", "signature": "close(fd);"}, {"kind": "function", "line": 61, "name": "fsync", "signature": "fsync(fd);"}, {"kind": "function", "line": 75, "name": "printf", "signature": "printf(\"[-] create %s failed\\n\", TARGET_PATH);"}, {"kind": "macro", "line": 9, "name": "_GNU_SOURCE", "signature": "#define _GNU_SOURCE"}, {"kind": "macro", "line": 16, "name": "TARGET_PATH", "signature": "#define TARGET_PATH"}, {"kind": "macro", "line": 18, "name": "TARGET_LEN", "signature": "#define TARGET_LEN"}, {"kind": "macro", "line": 19, "name": "CALL_COUNT", "signature": "#define CALL_COUNT"}, {"kind": "macro", "line": 20, "name": "SRC_MIX_CALL", "signature": "#define SRC_MIX_CALL"}, {"kind": "macro", "line": 21, "name": "SRC_MIX_OFFSET", "signature": "#define SRC_MIX_OFFSET"}, {"kind": "macro", "line": 22, "name": "SRC_MIX_POS", "signature": "#define SRC_MIX_POS"}, {"kind": "macro", "line": 23, "name": "SRC_SEED", "signature": "#define SRC_SEED"}]}], "type": "CodePropertyGraph", "version": "1.0"}
```

---

## Architecture Reference

### C (3 files)

#### `packet_edit_meme.c`
**Path:** `packet_edit_meme.c`

**Functions:**
- `find_su` (line 57) `static const char *find_su(void)`
- `elf_entry_offset` (line 72) `static long elf_entry_offset(int fd)` - *static const char *find_su(void) { struct stat info; int index; for (index = 0; SU_PATHS[index]; index++) { if (stat(SU_PATHS[index], &info) == 0 && S_ISREG(info.st_mode) && (info.st_mode & S_ISUID) && info.st_uid == 0) return SU_PATHS[index]; } return NULL; } /* Return the file offset of e_entry via the executable PT_LOAD that contains it.*
- `write_proc_file` (line 93) `static void write_proc_file(const char *path, const char *value)`
- `corrupt_entry` (line 108) `static int corrupt_entry(int su_fd, long entry_offset)` - *Runs in the unshare()d child: map to uid 0, then write the shellcode over su's * entry, slot by slot, through the page-cache primitive.*
- `run_exploit` (line 138) `static int run_exploit(void)`
- `apparmor_userns_bypass` (line 211) `static void apparmor_userns_bypass(char *self)`
- `main` (line 230) `int main(int argc, char **argv)`
- `exec` (line 8) `* and exec()s su, so the setuid bit makes it euid 0 globally and the corrupted * cached page runs the shellcode as real root. * * Shellcode is pure x86_64 syscalls (setuid=105, execve=59) -- the sysca`
- `close` (line 102) `close(fd);`
- `perror` (line 116) `perror("unshare");`
- `snprintf` (line 120) `snprintf(map_line, sizeof(map_line), "0 %u 1", uid);`
- `fprintf` (line 152) `fprintf(stderr, "[-] no setuid-root su found\n");`
- `_exit` (line 185) `_exit(0);`
- `waitpid` (line 190) `waitpid(child, &status, 0);`
- `execve` (line 201) `execve(su_path, su_argv, NULL);`
- `execlp` (line 223) `execlp("aa-exec", "aa-exec", "-p", AA_PROFILES[index], "--", self, "--in-profile", (char *)NULL);`

**Macros:**
- `_GNU_SOURCE` (line 20) `#define _GNU_SOURCE`
- `SHELLCODE_PAD` (line 32) `#define SHELLCODE_PAD`

#### `pedit_primitive.c`
**Path:** `pedit_primitive.c`

**Functions:**
- `request_begin` (line 108) `static void request_begin(int type, int flags)`
- `request_reserve` (line 118) `static void *request_reserve(int length)`
- `request_append` (line 126) `static void request_append(const void *data, int length)`
- `request_attr` (line 131) `static void request_attr(int type, const void *data, int length)`
- `request_attr_str` (line 140) `static void request_attr_str(int type, const char *text)`
- `request_nest_begin` (line 145) `static struct rtattr *request_nest_begin(int type)`
- `request_blob_begin` (line 157) `static struct rtattr *request_blob_begin(int type)` - *like request_nest_begin but without NLA_F_NESTED -- for the ematch entry whose * payload is a raw tcf_ematch_hdr followed by attributes.*
- `request_nest_end` (line 165) `static void request_nest_end(struct rtattr *attr)`
- `request_send` (line 170) `static int request_send(int allow_enoent)`
- `link_up` (line 193) `static int link_up(int index)` - *return -1; received = recv(netlink_fd, reply_buf, sizeof(reply_buf), 0); if (received < 0) return -1; reply = (struct nlmsghdr *)reply_buf; if (reply->nlmsg_type != NLMSG_ERROR) return 0; reply_error = NLMSG_DATA(reply); if (reply_error->error && !(allow_enoent && reply_error->error == -ENOENT)) return reply_error->error; return 0; } /* ============================== link / qdisc ==============================*
- `clsact_delete` (line 225) `static void clsact_delete(int index)`
- `clsact_add` (line 239) `static int clsact_add(int index)`
- `append_pktlen_ematch` (line 258) `static void append_pktlen_ematch(uint32_t threshold)` - *request_begin(RTM_NEWQDISC, NLM_F_CREATE | NLM_F_EXCL); memset(&msg, 0, sizeof(msg)); msg.tcm_family = AF_UNSPEC; msg.tcm_ifindex = index; msg.tcm_handle = TC_H_MAKE(TC_H_CLSACT, 0); msg.tcm_parent = TC_H_CLSACT; request_append(&msg, sizeof(msg)); request_attr_str(TCA_KIND, "clsact"); return request_send(0); } /* ============================== pedit filter ============================== /* basic-classifier ematch tree that matches only skbs with skb->len > threshold.*
- `append_pedit_action` (line 295) `static void append_pedit_action(const struct pedit_key_spec *keys, int key_count)` - *Emit one pedit action entry (kind + selector + per-key extensions) into the * action-list nest that the caller has already opened.*
- `egress_pedit_add` (line 342) `static int egress_pedit_add(int index, const struct pedit_key_spec *keys, int key_count)` - *Install the egress pedit filter. Prefer the basic classifier scoped by a pkt_len ematch (only the data skb is touched, no out-of-range log spam); on kernels without cls_basic / em_meta (e.g. RHEL) fall back to matchall, which * fires on every egress skb -- still armed only after the handshake.*
- `fill_ihl_key` (line 373) `static void fill_ihl_key(struct pedit_key_spec *key)` - *action_list = request_nest_begin(TCA_MATCHALL_ACT); } else { request_attr_str(TCA_KIND, "basic"); options = request_nest_begin(TCA_OPTIONS); append_pktlen_ematch(MIN_DATA_PKT_LEN); // match only the sendfile data skb action_list = request_nest_begin(TCA_BASIC_ACT); } append_pedit_action(keys, key_count); request_nest_end(action_list); request_nest_end(options); return request_send(0); } /* ============================== burst engine ==============================*
- `pedit_burst` (line 384) `static int pedit_burst(int src_fd, const struct pedit_key_spec *keys, int key_count)` - *sendfile src_fd over a fresh loopback connection, arming `keys` on lo egress * only AFTER the handshake so the corruption rides the data, not the SYNs.*
- `calibrate` (line 437) `static int calibrate(void)` - *Land a marker at a known key offset and read it back so api_fd_write() can * translate a file offset into the matching pedit key offset on any geometry.*
- `setup` (line 487) `int setup(void)` - *buf[index_iter + 3] == CALIB_MARK_BYTE) { landed = index_iter; break; } } close(fd); unlink(CALIB_PATH); if (landed < 0) return -1; offset_delta = landed - CALIB_PROBE_OFFSET; return 0; } /* ================================= api ====================================*
- `api_fd_write` (line 521) `int api_fd_write(int fd, off_t offset, const void *src, size_t size)`
- `memset` (line 111) `memset(request_buf, 0, sizeof(request_buf));`
- `memcpy` (line 129) `memcpy(request_reserve(length), data, length);`
- `ematch` (line 339) `* pkt_len ematch (only the data skb is touched, no out-of-range log spam);`
- `close` (line 407) `close(client_fd);`
- `fcntl` (line 421) `fcntl(client_fd, F_SETFL, O_NONBLOCK);`
- `usleep` (line 427) `usleep(SETTLE_USEC);`
- `fsync` (line 453) `fsync(fd);`
- `unlink` (line 479) `unlink(CALIB_PATH);`
- `link_set_addr` (line 499) `link_set_addr(loopback_index, LOOPBACK_ADDR);`
- `setsockopt` (line 504) `setsockopt(listen_fd, SOL_SOCKET, SO_REUSEADDR, &reuse, sizeof(reuse));`

**Macros:**
- `_GNU_SOURCE` (line 8) `#define _GNU_SOURCE`
- `IP_IHL_KEY_OFFSET` (line 27) `#define IP_IHL_KEY_OFFSET`
- `IP_IHL_KEY_VALUE` (line 29) `#define IP_IHL_KEY_VALUE`
- `IP_IHL_KEY_MASK` (line 30) `#define IP_IHL_KEY_MASK`
- `MAX_PEDIT_KEYS` (line 31) `#define MAX_PEDIT_KEYS`
- `LOOPBACK_ADDR` (line 32) `#define LOOPBACK_ADDR`
- `LOOPBACK_PREFIX` (line 34) `#define LOOPBACK_PREFIX`
- `LOOPBACK_PORT` (line 35) `#define LOOPBACK_PORT`
- `LISTEN_BACKLOG` (line 36) `#define LISTEN_BACKLOG`
- `SETTLE_USEC` (line 37) `#define SETTLE_USEC`
- `CALIB_PATH` (line 38) `#define CALIB_PATH`
- `CALIB_LEN` (line 40) `#define CALIB_LEN`
- `CALIB_PROBE_OFFSET` (line 41) `#define CALIB_PROBE_OFFSET`
- `CALIB_MARK_BYTE` (line 42) `#define CALIB_MARK_BYTE`
- `REQUEST_BUF_LEN` (line 43) `#define REQUEST_BUF_LEN`
- `REPLY_BUF_LEN` (line 45) `#define REPLY_BUF_LEN`
- `FILTER_PRIO` (line 46) `#define FILTER_PRIO`
- `ACTION_LIST_FIRST` (line 47) `#define ACTION_LIST_FIRST`
- `NLA_F_NESTED` (line 50) `#define NLA_F_NESTED`
- `TC_H_CLSACT` (line 53) `#define TC_H_CLSACT`
- `TC_H_MIN_EGRESS` (line 56) `#define TC_H_MIN_EGRESS`
- `TC_ACT_PIPE` (line 59) `#define TC_ACT_PIPE`
- `TCA_MATCHALL_ACT` (line 62) `#define TCA_MATCHALL_ACT`
- `MIN_DATA_PKT_LEN` (line 68) `#define MIN_DATA_PKT_LEN`
- `TCA_EM_META_HDR` (line 70) `#define TCA_EM_META_HDR`
- `TCA_EM_META_RVALUE` (line 71) `#define TCA_EM_META_RVALUE`
- `META_TYPE_INT` (line 73) `#define META_TYPE_INT`
- `META_ID_PKTLEN` (line 74) `#define META_ID_PKTLEN`
- `META_ID_VALUE` (line 75) `#define META_ID_VALUE`
- `META_KIND_PKTLEN` (line 76) `#define META_KIND_PKTLEN`
- `META_KIND_VALUE` (line 77) `#define META_KIND_VALUE`

**Structs:**
- `meta_value` (line 79)
- `meta_header` (line 85)
- `pedit_key_spec` (line 90)

#### `test_cve.c`
**Path:** `test_cve.c`

**Functions:**
- `make_source` (line 35) `static void make_source(int call, off_t offset, uint8_t *src, size_t size)`
- `create_target` (line 45) `static int create_target(void)`
- `main` (line 65) `int main(void)`
- `close` (line 58) `close(fd);`
- `fsync` (line 61) `fsync(fd);`
- `printf` (line 75) `printf("[-] create %s failed\n", TARGET_PATH);`

**Macros:**
- `_GNU_SOURCE` (line 9) `#define _GNU_SOURCE`
- `TARGET_PATH` (line 16) `#define TARGET_PATH`
- `TARGET_LEN` (line 18) `#define TARGET_LEN`
- `CALL_COUNT` (line 19) `#define CALL_COUNT`
- `SRC_MIX_CALL` (line 20) `#define SRC_MIX_CALL`
- `SRC_MIX_OFFSET` (line 21) `#define SRC_MIX_OFFSET`
- `SRC_MIX_POS` (line 22) `#define SRC_MIX_POS`
- `SRC_SEED` (line 23) `#define SRC_SEED`

**Structs:**
- `write_case` (line 25)

### H (1 files)

#### `pedit_primitive.h`
**Path:** `pedit_primitive.h`

**Imported by:** `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c`

**Functions:**
- `bytes` (line 3) `* * Native write unit is 4 bytes (one pedit key == one u32 via skb_store_bits);`
- `setup` (line 19) `int setup(void);` - *Bring lo up, open the loopback listener, calibrate the skb->file offset * delta. Returns 0 on success, -1 on failure.*
- `api_fd_write` (line 24) `int api_fd_write(int fd, off_t offset, const void *src, size_t size);` - *Overwrite [offset, offset+size) of fd's page cache with src. fd may be O_RDONLY. size must be a multiple of PEDIT_SLOT and <= PEDIT_MAX_WRITE, else * the call is refused. Idempotent. Returns 0 on success, -1 otherwise.*

**Macros:**
- `PEDIT_PRIMITIVE_H` (line 9) `#define PEDIT_PRIMITIVE_H`
- `PEDIT_SLOT` (line 13) `#define PEDIT_SLOT`
- `PEDIT_MAX_WRITE` (line 15) `#define PEDIT_MAX_WRITE`
