# Palette Library

Use this file when the user needs explicit hex-coded color systems for single-cell figures.

These palettes are designed for:

- stable reuse across many panels
- reduced visual noise compared with random category palettes
- practical support for `7-80` subtypes
- compatibility with the base `nature-figure` hero colors

## 1. Core anchor palette

Use this small set for binary or low-cardinality condition displays:

```python
CORE_PALETTE = {
    "blue_main": "#0F4D92",
    "blue_secondary": "#3775BA",
    "green_1": "#DDF3DE",
    "green_2": "#AADCA9",
    "green_3": "#8BCF8B",
    "red_1": "#F6CFCB",
    "red_2": "#E9A6A1",
    "red_strong": "#B64342",
    "neutral_light": "#CFCECE",
    "neutral_mid": "#767676",
    "neutral_dark": "#4D4D4D",
    "neutral_black": "#272727",
    "gold": "#FFD700",
    "teal": "#42949E",
    "violet": "#9A4D8E",
    "magenta": "#EA84DD",
}
```

## 2. Default 24-color atlas palette

Use when:

- major lineages plus subtype-level views
- medium-cardinality cluster maps
- dotplots and composition figures that need color carryover from UMAP

```python
ATLAS24 = [
    "#0F4D92", "#3775BA", "#6EA6D9", "#AFCBE8",
    "#1E6F78", "#42949E", "#73B9B9", "#ABD6D3",
    "#2E7D4F", "#5BA36A", "#8BCF8B", "#BFE5B3",
    "#8A6D1F", "#C49A2C", "#E4C35A", "#F2DFA2",
    "#A14B2B", "#D97A33", "#EEA463", "#F6C8A0",
    "#9A4D8E", "#C45AD6", "#DEA0E8", "#EFC9F3",
]
```

Design logic:

- 6 hue families
- 4 lightness levels per family
- easier to visually group related states

## 3. Default 80-color large subtype palette

Use when:

- large fibroblast, myeloid, T/NK, endothelial, or pan-cancer atlases
- the user has `50-80` clusters and needs a stable starting point

```python
ATLAS80 = [
    "#254674", "#2C548C", "#3362A3", "#3B70BA", "#4D80C7", "#6A91C8", "#80A2D0", "#97B2D8",
    "#256774", "#2C7C8C", "#3390A3", "#3BA5BA", "#4DB2C7", "#6AB8C8", "#80C3D0", "#97CDD8",
    "#257464", "#2C8C78", "#33A38D", "#3BBAA1", "#4DC7AE", "#6AC8B5", "#80D0C0", "#97D8CB",
    "#25742B", "#2C8C34", "#33A33D", "#3BBA45", "#4DC757", "#6AC872", "#80D087", "#97D89C",
    "#577425", "#698C2C", "#7AA333", "#8BBA3B", "#9AC74D", "#A6C86A", "#B3D080", "#C0D897",
    "#746025", "#8C742C", "#A38733", "#BA9A3B", "#C7A84D", "#C8B06A", "#D0BC80", "#D8C897",
    "#744525", "#8C522C", "#A36033", "#BA6E3B", "#C77E4D", "#C8906A", "#D0A080", "#D8B197",
    "#742A25", "#8C322C", "#A33B33", "#BA433B", "#C7554D", "#C8706A", "#D08680", "#D89B97",
    "#742542", "#8C2C4F", "#A3335C", "#BA3B69", "#C74D79", "#C86A8C", "#D0809E", "#D897AF",
    "#572574", "#692C8C", "#7A33A3", "#8B3BBA", "#9A4DC7", "#A66AC8", "#B380D0", "#C097D8",
]
```

Design logic:

- 10 hue families
- 8 shades per family
- practical when subclusters are grouped hierarchically

Recommended use:

- assign one family to one major lineage, then shades to its subclusters
- do not randomly shuffle unless you intentionally want family information hidden

## 4. Binary and low-cardinality condition sets

```python
RESPONSE_BINARY = ["#272727", "#B64342"]
PRE_POST = ["#4D4D4D", "#3775BA", "#D97A33"]
TUMOR_NORMAL_MET = ["#42949E", "#B64342", "#9A4D8E"]
SPATIAL_OVERLAY = ["#000000", "#22D7E6", "#FF2AD4", "#FFFFFF"]
```

## 5. Practical usage rules

- If cell types are reused across UMAP, composition, and dotplot panels, lock the same mapping.
- For manuscript-wide consistency, save the mapping as a table or dictionary instead of rebuilding it ad hoc.
- If a cluster family is visually too similar for a small panel, collapse to a coarser lineage palette rather than randomizing all colors.

## 6. Why these palettes exist

The reference literature repeatedly uses:

- restrained, family-structured colors
- consistent condition mapping across panels
- spatial overlays with black background and 1-2 fluorescent accents

This file turns that implicit practice into explicit hex-coded defaults.
