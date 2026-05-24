# Parameter Defaults

These defaults come from the supplied Scanpy pipeline and are starting points, not universal truths.

## QC

- `min_genes = 300`
- `max_genes = 6000`
- `min_counts = 500`
- `max_counts = 60000`
- `min_cells = 50`
- `mito_thresh = 15`

## Integration and clustering

- `batch_method = bbknn`
- `n_top_genes = 2500`
- `n_pcs = 50`
- `n_neighbors = 20`
- `bbknn_n_pcs = 50`
- `neighbors_within_batch = 3`
- `resolution = 1.0`

## Score and export

- `score_methods = score_genes,mean_expr,mean_z`
- `score_dpi = 300`
- `figure_dpi = 300`

## When to deviate

- nuclei or fragile tissues -> relax RNA-content thresholds
- very large multi-dataset integration -> consider `scVI`
- response papers -> add patient-aware DE and proportion exports
- malignant compartment studies -> add CNV branch
