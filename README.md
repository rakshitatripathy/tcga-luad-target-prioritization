# TCGA LUAD Gene Expression Analysis (PCA)

## Overview
This project analyzes RNA-seq gene expression data from The Cancer Genome Atlas (TCGA) Lung Adenocarcinoma (LUAD) dataset. The goal was to explore differences between tumor and normal samples. Gene expression counts were processed into a unified matrix, standardized, and reduced using PCA. The results show partial separation between tumor and normal samples indicating differences in gene expression while reflecting biological heterogenity. 

## Data
- Source: TCGA LUAD (Genomic Data Commons)
- Type: RNA-seq gene expression counts 
- Format: TSV files (STAR output)
- Samples: 100 total (50 tumor, 50 normal)

## Methods
- Analyzed gene expression files and extracted relevant columns 
- Removed non-gene rows
- Merged all samples into single gene expression matrix
- Transposed data (samples x genes)
- Standarized features using 'StandardScaler'
- Applied Principal Component Analysis (PCA), a dimensionality reduction technique that summarizes variation across thousands of genes into a few components

## Results
- PCA reveals separation between tumor and normal samples 
- Indicates differences in gene expression patterns
- Overlap suggests biological variability between samples

## Files
- `analysis.ipynb` → main analysis notebook  
- `pca_with_metadata.csv` → PCA results with sample labels  
- `pca_plot.png` → visualization of PCA  

## Tools
- Python
- Pandas
- Numpy
- Matplotlib
- Scikit-learn

## Takeaways
- Built a full RNA-seq preprocessing and anlysis pipeline
- Demonstrated how PCA can reveal structire in biologicla data
- Highlighted gene expression differences in cancer vs normal tissue

## Author
Rakshita Tripathy
B.S. Biology, UC Riverside (Class of 2026)


