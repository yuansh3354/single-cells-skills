---
name: single-cell-methods
description: >-
  Plan and adapt single-cell analysis workflows for scRNA-seq, snRNA-seq, and single-cell-plus-spatial
  studies using literature-derived method stacks, parameter defaults, and task-specific recipes.
  Use when the user asks which methods to use, how to set parameters, how to extend a Scanpy pipeline,
  or how to handle special cases such as response analysis, trajectory inference, CNV, spatial mapping,
  cell-cell communication, or clonality.
---

# Single-Cell Methods

Use this skill when the main task is choosing or structuring analysis methods.

This skill is grounded in the user's supplied Scanpy pipeline plus repeated methods found across the
provided literature corpus.

## Open these files

| File | Open when |
|---|---|
| [references/core-workflow.md](references/core-workflow.md) | You need the baseline single-cell workflow |
| [references/task-recipes.md](references/task-recipes.md) | You need task-specific method combinations |
| [references/parameter-defaults.md](references/parameter-defaults.md) | You need parameter defaults and when to deviate |
| [references/special-cases.md](references/special-cases.md) | You need less standard or paper-specific extensions |
| [references/source-basis.md](references/source-basis.md) | You need to see which literature patterns informed the methods skill |

## Core rules

- Choose methods from the biological question, not from tool popularity.
- Do not add trajectory, communication, CNV, or spatial mapping unless they feed a real claim.
- Keep patient-level inference separate from pooled cell-level summaries.
- Preserve the strengths of the existing pipeline instead of replacing it for cosmetic reasons.
