# Concepts

Nouns map atomically to file sets (EXTRACTED); verbs aggregate structural edges (INFERRED).

- `offset` | files=4 | mentions=11 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h`, `test_cve.c`
- `write` | files=4 | mentions=8 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h`, `test_cve.c`
- `primitive` | files=3 | mentions=6 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h`
- `file` | files=3 | mentions=4 | `packet_edit_meme.c`, `pedit_primitive.c`, `pedit_primitive.h`
- `source` | files=3 | mentions=4 | `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c`
- `gnu` | files=3 | mentions=3 | `packet_edit_meme.c`, `pedit_primitive.c`, `test_cve.c`
- `pedit` | files=2 | mentions=18 | `pedit_primitive.c`, `pedit_primitive.h`
- `index` | files=2 | mentions=7 | `packet_edit_meme.c`, `pedit_primitive.c`
- `len` | files=2 | mentions=7 | `pedit_primitive.c`, `test_cve.c`
- `entry` | files=2 | mentions=6 | `packet_edit_meme.c`, `pedit_primitive.c`
- `loopback` | files=2 | mentions=5 | `pedit_primitive.c`, `pedit_primitive.h`
- `return` | files=2 | mentions=4 | `packet_edit_meme.c`, `pedit_primitive.c`
- `skb` | files=2 | mentions=4 | `pedit_primitive.c`, `pedit_primitive.h`
- `slot` | files=2 | mentions=4 | `packet_edit_meme.c`, `pedit_primitive.h`
- `api` | files=2 | mentions=3 | `pedit_primitive.c`, `pedit_primitive.h`
- `call` | files=2 | mentions=3 | `pedit_primitive.h`, `test_cve.c`
- `max` | files=2 | mentions=3 | `pedit_primitive.c`, `pedit_primitive.h`
- `cache` | files=2 | mentions=2 | `packet_edit_meme.c`, `pedit_primitive.h`
- `calibrate` | files=2 | mentions=2 | `pedit_primitive.c`, `pedit_primitive.h`
- `create` | files=2 | mentions=2 | `pedit_primitive.c`, `test_cve.c`
- `int` | files=2 | mentions=2 | `packet_edit_meme.c`, `pedit_primitive.c`
- `make` | files=2 | mentions=2 | `pedit_primitive.c`, `test_cve.c`
- `over` | files=2 | mentions=2 | `packet_edit_meme.c`, `pedit_primitive.c`
- `page` | files=2 | mentions=2 | `packet_edit_meme.c`, `pedit_primitive.h`
- `path` | files=2 | mentions=2 | `pedit_primitive.c`, `test_cve.c`
- `setup` | files=2 | mentions=2 | `pedit_primitive.c`, `pedit_primitive.h`

## Verb Edges

- `gnu` --consumes--> `api` (strength 1.00)
- `gnu` --depends_on--> `api` (strength 1.00)
- `gnu` --consumes--> `cache` (strength 1.00)
- `gnu` --depends_on--> `cache` (strength 1.00)
- `gnu` --consumes--> `calibrate` (strength 1.00)
- `gnu` --depends_on--> `calibrate` (strength 1.00)
- `gnu` --consumes--> `call` (strength 1.00)
- `gnu` --depends_on--> `call` (strength 1.00)
- `gnu` --consumes--> `file` (strength 1.00)
- `gnu` --depends_on--> `file` (strength 1.00)
- `gnu` --consumes--> `loopback` (strength 1.00)
- `gnu` --depends_on--> `loopback` (strength 1.00)
- `gnu` --consumes--> `max` (strength 1.00)
- `gnu` --depends_on--> `max` (strength 1.00)
- `gnu` --consumes--> `offset` (strength 1.00)
- `gnu` --depends_on--> `offset` (strength 1.00)
- `gnu` --consumes--> `page` (strength 1.00)
- `gnu` --depends_on--> `page` (strength 1.00)
- `gnu` --consumes--> `pedit` (strength 1.00)
- `gnu` --depends_on--> `pedit` (strength 1.00)
- `gnu` --consumes--> `primitive` (strength 1.00)
- `gnu` --depends_on--> `primitive` (strength 1.00)
- `gnu` --consumes--> `setup` (strength 1.00)
- `gnu` --depends_on--> `setup` (strength 1.00)
- `gnu` --consumes--> `skb` (strength 1.00)
- `gnu` --depends_on--> `skb` (strength 1.00)
- `gnu` --consumes--> `slot` (strength 1.00)
- `gnu` --depends_on--> `slot` (strength 1.00)
- `gnu` --consumes--> `write` (strength 1.00)
- `gnu` --depends_on--> `write` (strength 1.00)
- `offset` --consumes--> `api` (strength 1.00)
- `offset` --depends_on--> `api` (strength 1.00)
- `offset` --consumes--> `cache` (strength 1.00)
- `offset` --depends_on--> `cache` (strength 1.00)
- `offset` --consumes--> `calibrate` (strength 1.00)
- `offset` --depends_on--> `calibrate` (strength 1.00)
- `offset` --consumes--> `call` (strength 1.00)
- `offset` --depends_on--> `call` (strength 1.00)
- `offset` --consumes--> `file` (strength 1.00)
- `offset` --depends_on--> `file` (strength 1.00)
- `offset` --consumes--> `loopback` (strength 1.00)
- `offset` --depends_on--> `loopback` (strength 1.00)
- `offset` --consumes--> `max` (strength 1.00)
- `offset` --depends_on--> `max` (strength 1.00)
- `offset` --consumes--> `page` (strength 1.00)
- `offset` --depends_on--> `page` (strength 1.00)
- `offset` --consumes--> `pedit` (strength 1.00)
- `offset` --depends_on--> `pedit` (strength 1.00)
- `offset` --consumes--> `primitive` (strength 1.00)
- `offset` --depends_on--> `primitive` (strength 1.00)

## Dialectic

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
