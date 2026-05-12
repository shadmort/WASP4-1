# WASP4-1
Wyss Analysis Software for Proteomics; LFQ-DIA

A data processing pipeline for PEAKS output.

Input:
  - PEAKS peptide-level quantification
  - Annotation file

Procedure:
  - Data wrangling
  - Completeness filter 50% in one group
  - Log2 transform
  - QRILC-style imputation
  - Median normalization
  - Peptide intensity filter
  - Intragroup CV filter
  - Protein summary by Tukey's median polish
  - Removal of ambiguous peptides
  - Removal of single peptide-protein hits
  - Data

Returns:
  - Pre-norm RLE plot
  - Imputation histogram
  - PCA
  - UMAP
  - Filtered peptide matrix
  - Aggregated protein matrix
  - Single-peptide proteins
