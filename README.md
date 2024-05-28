# RNAseq-pipeline-using-Nextflow-of-EGFL1-Over-expression-in-Cervical-Cancer-Tissue
# RNA-seq Pipeline with Nextflow

This repository contains a Nextflow pipeline for processing RNA sequencing (RNA-seq) data. The pipeline performs the following steps:

1. **Quality Control:** Using FastQC and Trimmomatic for quality assessment and trimming of low-quality reads.
2. **Read Alignment:** Aligning trimmed reads to the human reference genome (GRCh38) using HISAT2.
3. **Read Quantification:** Quantifying gene expression levels using featureCounts.

## Pipeline Features:

- **Reproducible:** The pipeline is built using Nextflow, a workflow management system that ensures reproducibility and portability.
- **Efficient:** Utilizes parallel processing where possible to optimize performance.
- **Easy to Use:**  The pipeline can be easily customized and run with different parameters.

## Getting Started:

1. **Clone this repository:**
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
