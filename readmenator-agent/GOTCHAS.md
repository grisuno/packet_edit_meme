# Gotchas

## God Nodes (high connectivity)

These files have the most connections. Changes here have high blast radius.

- `pedit_primitive.c` (score: 7.50)
- `pedit_primitive.h` (score: 6.60, imported by 3 files)
- `packet_edit_meme.c` (score: 3.00)

## Blast Radius (change impact)

Editing these files can break the listed number of dependents. Run their tests after any change.

- `pedit_primitive.h` -- 3 direct, 3 total dependents

## Hotspots (complexity + centrality)

- `pedit_primitive.c` -- complexity: 1.0, centrality: 1.0, combined: 1.0
- `packet_edit_meme.c` -- complexity: 0.2, centrality: 0.6, combined: 0.5
- `pedit_primitive.h` -- complexity: 0.1, centrality: 0.4, combined: 0.3
