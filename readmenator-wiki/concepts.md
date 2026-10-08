# Concepts

Second-brain semantic layer: nouns map atomically to file sets (EXTRACTED); verbs aggregate structural edges (INFERRED).

| Concept | Files | Mentions | Top Files |
|---------|-------|----------|-----------|
| `offset` | 4 | 11 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h`, `test_cve.c` |
| `write` | 4 | 8 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h`, `test_cve.c` |
| `primitive` | 3 | 6 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h` |
| `file` | 3 | 4 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h` |
| `source` | 3 | 4 | `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c` |
| `gnu` | 3 | 3 | `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c` |
| `pedit` | 2 | 18 | `pedit_primitive.c`, `pedit_primitive.h` |
| `index` | 2 | 7 | `packet_edit_meme.c`, `pedit_primitive.c` |
| `len` | 2 | 7 | `pedit_primitive.c`, `test_cve.c` |
| `entry` | 2 | 6 | `packet_edit_meme.c`, `pedit_primitive.c` |
| `loopback` | 2 | 5 | `pedit_primitive.c`, `pedit_primitive.h` |
| `return` | 2 | 4 | `packet_edit_meme.c`, `pedit_primitive.c` |
| `skb` | 2 | 4 | `pedit_primitive.c`, `pedit_primitive.h` |
| `slot` | 2 | 4 | `packet_edit_meme.c`, `pedit_primitive.h` |
| `api` | 2 | 3 | `pedit_primitive.c`, `pedit_primitive.h` |
| `call` | 2 | 3 | `pedit_primitive.h`, `test_cve.c` |
| `max` | 2 | 3 | `pedit_primitive.c`, `pedit_primitive.h` |
| `cache` | 2 | 2 | `packet_edit_meme.c`, `pedit_primitive.h` |
| `calibrate` | 2 | 2 | `pedit_primitive.c`, `pedit_primitive.h` |
| `create` | 2 | 2 | `pedit_primitive.c`, `test_cve.c` |
| `int` | 2 | 2 | `packet_edit_meme.c`, `pedit_primitive.c` |
| `make` | 2 | 2 | `pedit_primitive.c`, `test_cve.c` |
| `over` | 2 | 2 | `packet_edit_meme.c`, `pedit_primitive.c` |
| `page` | 2 | 2 | `packet_edit_meme.c`, `pedit_primitive.h` |
| `path` | 2 | 2 | `pedit_primitive.c`, `test_cve.c` |
| `setup` | 2 | 2 | `pedit_primitive.c`, `pedit_primitive.h` |

## Verb Edges

| Source | Verb | Target | Strength |
|--------|------|--------|----------|
| `gnu` | `consumes` | `api` | 1.00 |
| `gnu` | `depends_on` | `api` | 1.00 |
| `gnu` | `consumes` | `cache` | 1.00 |
| `gnu` | `depends_on` | `cache` | 1.00 |
| `gnu` | `consumes` | `calibrate` | 1.00 |
| `gnu` | `depends_on` | `calibrate` | 1.00 |
| `gnu` | `consumes` | `call` | 1.00 |
| `gnu` | `depends_on` | `call` | 1.00 |
| `gnu` | `consumes` | `file` | 1.00 |
| `gnu` | `depends_on` | `file` | 1.00 |
| `gnu` | `consumes` | `loopback` | 1.00 |
| `gnu` | `depends_on` | `loopback` | 1.00 |
| `gnu` | `consumes` | `max` | 1.00 |
| `gnu` | `depends_on` | `max` | 1.00 |
| `gnu` | `consumes` | `offset` | 1.00 |
| `gnu` | `depends_on` | `offset` | 1.00 |
| `gnu` | `consumes` | `page` | 1.00 |
| `gnu` | `depends_on` | `page` | 1.00 |
| `gnu` | `consumes` | `pedit` | 1.00 |
| `gnu` | `depends_on` | `pedit` | 1.00 |
| `gnu` | `consumes` | `primitive` | 1.00 |
| `gnu` | `depends_on` | `primitive` | 1.00 |
| `gnu` | `consumes` | `setup` | 1.00 |
| `gnu` | `depends_on` | `setup` | 1.00 |
| `gnu` | `consumes` | `skb` | 1.00 |
| `gnu` | `depends_on` | `skb` | 1.00 |
| `gnu` | `consumes` | `slot` | 1.00 |
| `gnu` | `depends_on` | `slot` | 1.00 |
| `gnu` | `consumes` | `write` | 1.00 |
| `gnu` | `depends_on` | `write` | 1.00 |
| `offset` | `consumes` | `api` | 1.00 |
| `offset` | `depends_on` | `api` | 1.00 |
| `offset` | `consumes` | `cache` | 1.00 |
| `offset` | `depends_on` | `cache` | 1.00 |
| `offset` | `consumes` | `calibrate` | 1.00 |
| `offset` | `depends_on` | `calibrate` | 1.00 |
| `offset` | `consumes` | `call` | 1.00 |
| `offset` | `depends_on` | `call` | 1.00 |
| `offset` | `consumes` | `file` | 1.00 |
| `offset` | `depends_on` | `file` | 1.00 |
| `offset` | `consumes` | `loopback` | 1.00 |
| `offset` | `depends_on` | `loopback` | 1.00 |
| `offset` | `consumes` | `max` | 1.00 |
| `offset` | `depends_on` | `max` | 1.00 |
| `offset` | `consumes` | `page` | 1.00 |
| `offset` | `depends_on` | `page` | 1.00 |
| `offset` | `consumes` | `pedit` | 1.00 |
| `offset` | `depends_on` | `pedit` | 1.00 |
| `offset` | `consumes` | `primitive` | 1.00 |
| `offset` | `depends_on` | `primitive` | 1.00 |

## Dialectic Prompts

- Thesis: `api` centralizes 2 files; Antithesis: `calibrate` pulls 2 files with 2 shared (Jaccard 1.00); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `file` pulls 3 files with 2 shared (Jaccard 0.67); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `loopback` pulls 2 files with 2 shared (Jaccard 1.00); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `max` pulls 2 files with 2 shared (Jaccard 1.00); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `offset` pulls 4 files with 2 shared (Jaccard 0.50); Synthesis: should they merge, split by layer, or keep `consumes` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `pedit` pulls 2 files with 2 shared (Jaccard 1.00); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `primitive` pulls 3 files with 2 shared (Jaccard 0.67); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `setup` pulls 2 files with 2 shared (Jaccard 1.00); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `skb` pulls 2 files with 2 shared (Jaccard 1.00); Synthesis: should they merge, split by layer, or keep `bridges` explicit?
- Thesis: `api` centralizes 2 files; Antithesis: `write` pulls 4 files with 2 shared (Jaccard 0.50); Synthesis: should they merge, split by layer, or keep `consumes` explicit?
