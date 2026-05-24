---
name: single-cell-figure
description: >-
  Build publication-grade single-cell figures for scRNA-seq, snRNA-seq, and single-cell-plus-spatial
  studies, with explicit large-scale discrete palettes, stable cell-type color systems, atlas and
  response figure archetypes, and journal-ready panel logic. Use when the user asks for UMAP,
  dotplot, heatmap, composition, pathway, spatial, trajectory, or multi-panel single-cell figures,
  especially when many cell states require reusable hex-coded palettes.
---

# Single-Cell Figure

Use this skill when the main task is figure planning, plotting, color selection, or panel logic for
single-cell papers.

This skill explicitly borrows figure contract, typography, SVG, and panel hierarchy logic from
`nature-figure`, but extends it for the specific pain points of single-cell plotting:

- too many clusters
- unstable colors across panels
- no distinction between atlas, response, spatial, and trajectory figure logic
- random categorical palettes that waste time and reduce readability

## Open these files

| File | Open when |
|---|---|
| [references/palette-library.md](references/palette-library.md) | You need explicit hex-coded palettes for 10, 24, 40, or 80 cluster scenarios |
| [references/figure-contract.md](references/figure-contract.md) | You need panel hierarchy, core-conclusion planning, or reviewer-risk framing |
| [references/figure-archetypes.md](references/figure-archetypes.md) | You need atlas, response, spatial, trajectory, or supplementary figure layouts |
| [references/style-rules.md](references/style-rules.md) | You need typography, export, UMAP, dotplot, heatmap, composition, and spatial panel rules |

## Core rules

- Keep one stable color for one biological identity across the whole manuscript.
- Use explicit hex-coded palettes, not default plotting-library category cycles.
- For large subtype atlases, use family-structured palettes rather than random hue jumps.
- Reserve red/green mainly for directional up/down signals unless the paper already established another mapping.
- Use SVG-first export when text or labels may need revision.
