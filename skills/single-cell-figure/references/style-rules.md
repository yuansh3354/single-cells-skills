# Style Rules

## Typography

```python
plt.rcParams['font.family'] = 'sans-serif'
plt.rcParams['font.sans-serif'] = ['Arial', 'DejaVu Sans', 'Liberation Sans']
plt.rcParams['svg.fonttype'] = 'none'
```

## Export

- primary: SVG
- secondary: PDF or PNG

## UMAP

- one large overview panel
- quieter companion panels
- avoid repeated equal-weight UMAPs

## Dotplot and heatmap

- use biological grouping
- keep cluster order stable
- do not dump every marker

## Composition

- always define denominator
- prefer patient-level comparisons where possible

## Spatial overlays

- black background only inside image plates
- use `SPATIAL_OVERLAY` colors when channels need explicit contrast
