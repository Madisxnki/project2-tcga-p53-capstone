# project2-tcga-p53-capstone
TCGA analysis of CCNB1 expression by TP53 status in lung adenocarcinoma.

# Does CCNB1 Expression Respond to p53 Loss?

This project examines whether CCNB1 expression differs according to TP53 mutation status in lung adenocarcinoma (LUAD), using tumour and normal tissue data from The Cancer Genome Atlas (TCGA).

## Assigned Gene and Cancer Type

The assigned gene is **CCNB1**, and the cancer type is **LUAD**.

## Notebooks

The analysis is organised into three notebooks, each covering a different part of the investigation.

- `01_cohort_table.ipynb` prepares the clinical data and summarises the patient cohort.
- `02_p53_analysis.ipynb` examines CCNB1 expression across cancer types before comparing TP53-mutant and wild-type tumours in LUAD.
- `03_extension.ipynb` explores whether similar differences in CCNB1 expression are found in other cancer types.

Open each notebook in Google Colab and save a copy to Google Drive before editing. Enter your Sussex username in the setup cell, then run the cells in order. Notebook 01 summarises the clinical cohort, while Notebook 02 analyses CCNB1 expression independently of Notebook 01. Notebook 03 is an optional extension that examines whether the TP53-associated expression pattern is also seen in other cancer types.

## Main Result

In LUAD, CCNB1 expression was higher in tumours carrying a TP53 mutation than in those with wild-type TP53. The median difference was 0.986 log₂ units (p = 2.62 × 10⁻¹³), suggesting a strong association between TP53 mutation status and increased CCNB1 expression. However, this does not show that TP53 loss directly causes the increase.

## Extension

We also examined whether this pattern appeared in other cancer types. Of the 12 cancer types with sufficient samples in both groups, 10 showed higher CCNB1 expression in TP53-mutant tumours, with unadjusted p-values below 0.05. LGG and COAD showed small differences in the opposite direction, although neither was statistically significant.

These findings suggest that the association between TP53 mutation and CCNB1 expression may extend beyond LUAD. However, because several comparisons were made without adjusting the p-values for multiple testing, the results should be treated as exploratory rather than evidence of a causal relationship.
