# Second Brain

*Last synthesized: 2026-10-07 | 4 files | 1 concept pages | offline, zero tokens*

> Raw sources -> readmenator wiki -> links (Karpathy LLM Wiki Pattern, deterministic).
> Start here, then open one community page. Prefer grep over full reads.

## Vault Overview

The codebase centres on `pedit_primitive.c`, `pedit_primitive.h`, `test_cve.c`. Architecturally it is 2 layers, dominant utility (3 files) across 1 import-based communities. Recorded risk surface: 0 security findings and 0 dependency cycles.

Communities are self-contained in the resolved import graph; no cross-boundary bridges were recorded.

Open work clusters around documentation (0% file coverage), 0 security findings, 0 taint paths, and 5 suggested exploration questions in `queries.md`.

## Stats

| Metric | Value |
|--------|-------|
| Files | 4 |
| Symbols | 83 |
| Resolved imports | 3 |
| Languages | c, h |
| Communities | 1 |
| Doc coverage | 0% (0/4 files) |
| Security findings | 0 |
| Estimated read cost | ~1313 tokens (chars/4, offline so $0) |

## Reading Order

1. Skim Stats and God Nodes below for blast radius.
2. Open the largest community page first, then follow Connections.
3. Use `queries.md` for the next question; log the answer there.

```
grep -rn '<keyword>' index.md community_*.md
readmenator query "<question>" --target readmenator_packet_edit_meme_7z4l_pq_
```

## Concept Wiki

- [root (4 files, cohesion 1.00)](./community_0_root.md)

## God Nodes

| File | Score |
|------|-------|
| `pedit_primitive.c` | 7.5 |
| `pedit_primitive.h` | 6.6 |
| `test_cve.c` | 3.2 |
| `packet_edit_meme.c` | 3.0 |

## Strongest Connections

- No cross-community connections recorded.

## Navigation Tips

- Obsidian Graph View works: every community page links back here.
- `connections.json` is machine-readable for GraphRAG pipelines.
- `REPORT.md` states what was extracted vs inferred and current limits.
- Regenerate offline: `readmenator . --rebuild` (no network, no tokens).
