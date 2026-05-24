# `single-cell` skill collection

A multi-skill collection for single-cell analysis, visualization, and manuscript writing.

This repository-style directory is designed around three separate but connected skills:

- `single-cell-figure`
- `single-cell-methods`
- `single-cell-writing`

The split is intentional:

- figure work needs explicit palette, panel, and export rules
- methods work needs task-layer method stacks, parameter defaults, and edge-case branches
- writing work needs evidence ladders, Methods structure, and bounded claims

## Directory structure

```text
single-cell/
├── README.md
├── PR_NOTES.md
├── README_PR_SNIPPET.md
└── skills/
    ├── single-cell-figure/
    ├── single-cell-methods/
    └── single-cell-writing/
```

## Included skills

### `single-cell-figure`

Focus:

- large-scale discrete palettes for 10, 24, and 80 cluster scenarios
- single-cell figure contract
- atlas / response / spatial / trajectory figure archetypes
- publication-grade export and typography

### `single-cell-methods`

Focus:

- literature-derived method combinations by task
- parameter defaults and when to deviate
- special-case analysis branches such as spatial mapping, CNV, trajectory, communication, and clonality
- adaptation of the provided Scanpy pipeline to paper-grade analysis

### `single-cell-writing`

Focus:

- Results evidence ladders
- module-based Methods writing
- figure legends and Discussion framing
- Chinese-note to English manuscript conversion

## Installation

For Codex, copy the subskills you want into `~/.codex/skills/`:

```bash
cp -R skills/single-cell-figure ~/.codex/skills/
cp -R skills/single-cell-methods ~/.codex/skills/
cp -R skills/single-cell-writing ~/.codex/skills/
```

## Reference bibliography

The collection was built from the user's provided paper set. Titles and DOI numbers are listed below.

| Title | DOI |
|---|---|
| A pan-cancer single-cell panorama of human natural killer cells | `10.1016/j.cell.2023.07.034` |
| A pan-cancer single-cell transcriptional atlas of tumor infiltrating myeloid cells | `10.1016/j.cell.2021.01.010` |
| A single-cell and spatial genomics atlas of human skin fibroblasts reveals shared disease-related fibroblast subtypes across tissue | `10.1038/s41590-025-02267-8` |
| A single-cell atlas reveals immune heterogeneity in anti-PD-1-treated non-small cell lung cancer | `10.1016/j.cell.2025.03.018` |
| A single-cell time-series atlas of endothelial cell embryonic development | `10.1016/j.cell.2026.01.002` |
| A spatially resolved atlas of gastric cancer characterises a lymphocyte-aggregated region | `10.1038/s41467-026-68612-z` |
| An SPP1-SOCS1 pathway constrains interferon responses in tumor-associated macrophages and shapes an immunosuppressive tumor microenvironment | `10.1016/j.immuni.2026.04.001` |
| An organotypic atlas of human vascular cells | `10.1038/s41591-024-03376-x` |
| COVID-19 immune features revealed by a large-scale single-cell transcriptome atlas | `10.1016/j.cell.2021.01.053` |
| Conserved spatial subtypes and cellular neighborhoods of cancer-associated fibroblasts revealed by single-cell spatial multi-omics | `10.1016/j.ccell.2025.03.004` |
| Cross-tissue human fibroblast atlas reveals myofibroblast subtypes with distinct roles in immune modulation | `10.1016/j.ccell.2024.08.020` |
| Distinct cellular mechanisms underlie chemotherapies and PD-L1 blockade combinations in triple-negative breast cancer | `10.1016/j.ccell.2025.01.007` |
| Evolution of immune and stromal cell states and ecotypes during gastric adenocarcinoma progression | `10.1016/j.ccell.2023.06.005` |
| Fibroblast atlas: Shared and specific cell types across tissues | `DOI not auto-resolved from local PDF; confirm manually before public release` |
| Immune phenotypic linkage between colorectal cancer and liver metastasis | `10.1016/j.ccell.2022.02.013` |
| Integrated single-cell and spatial transcriptomics uncover distinct cellular subtypes involved in neural invasion in pancreatic cancer | `10.1016/j.ccell.2025.06.020` |
| Integrated spatial transcriptomic profiling to dissect the cellular characteristics of tumor-associated tertiary lymphoid structures | `10.1016/j.celrep.2025.116250` |
| Landscape and Dynamics of Single Immune Cells in Hepatocellular Carcinoma | `10.1016/j.cell.2019.10.003` |
| Landscape of Infiltrating T Cells in Liver Cancer Revealed by Single-Cell Sequencing | `10.1016/j.cell.2017.05.035` |
| Liver tumour immune microenvironment subtypes and neutrophil heterogeneity | `10.1038/s41586-022-05400-x` |
| Multimodal clocks of human aging | `10.1016/j.cell.2026.04.025` |
| Multimodal spatial-omics reveal co-evolution of alveolar progenitors and proinflammatory niches in progression of lung precursor lesions | `10.1016/j.ccell.2025.10.004` |
| Oncogenic and tumor-suppressive forces converge on a progenitor niche at the benign-to-malignant transition | `10.1016/j.cell.2026.03.032` |
| Pan-cancer single-cell dissection reveals phenotypically distinct B cell subtypes | `10.1016/j.cell.2024.06.038` |
| Remodeling of T and endothelial cells during total neoadjuvant therapy in rectal cancer | `10.1016/j.ccell.2025.10.008` |
| Single cell T cell landscape and T cell receptor repertoire profiling of AML in context of PD-1 blockade therapy | `10.1038/s41467-021-26282-z` |
| Single cell clonotypic and transcriptional evolution of multiple myeloma precursor disease | `10.1016/j.ccell.2023.05.007` |
| Single-Cell Analyses Inform Mechanisms of Myeloid-Targeted Therapies in Colon Cancer | `10.1016/j.cell.2020.03.048` |
| Single-cell analyses reveal key immune cell subsets associated with response to PD-L1 blockade in triple-negative breast cancer | `10.1016/j.ccell.2021.09.010` |
| Single-cell screens identify ADAM12 as a fibroblast checkpoint impeding anti-tumor immunity | `10.1016/j.ccell.2025.12.018` |
| Spatiotemporal single-cell analysis decodes cellular dynamics underlying different responses to immunotherapy in colorectal cancer | `10.1016/j.ccell.2024.06.009` |

