# Special Cases

Use these only when the scientific question needs them.

## 1. Cross-platform integration

- 10x + SMART-seq2
- fresh tissue + FFPE/snRNA
- multi-center cohorts

Potential methods:

- `Harmony`
- `scVI`
- platform-aware validation after integration

## 2. Spatial niche discovery

- neighborhood vectors
- NMF-based niche decomposition
- spatially supported communication analysis

## 3. Personalized or paper-specific analysis

Examples seen across strong papers:

- response-group specific lineage re-clustering
- tissue-preference heatmaps
- cross-species alignment
- random-forest-assisted annotation
- logistic regression linking clinical metadata to response categories

These are not defaults, but they are valid when they match the study design.
