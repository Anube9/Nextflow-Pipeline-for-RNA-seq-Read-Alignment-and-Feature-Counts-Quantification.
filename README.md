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
   ```
2. **Install Nextflow:**
   Follow the instructions on the Nextflow website: [https://www.nextflow.io/docs/latest/getstarted.html](https://www.nextflow.io/docs/latest/getstarted.html)

3. **Download Required Data:**
   - **Reference Genome:** Download the HISAT2 index for GRCh38 (adjust the path in `params.genome_index` accordingly).
   - **GTF Annotation File:** Download the GTF file for GRCh38 (adjust the path in `params.gtf_file` accordingly).
   - **RNA-seq Reads:** Place your paired-end FASTQ files (named with the pattern `*_R{1,2}.fastq.gz`) in the `data` directory.

4. **Run the Pipeline:**
   ```bash
   cd rnaseq-pipeline
   nextflow run rnaseq_pipeline.nf
   ```

5. **Results:** The output files will be located in the `results` directory.

## Customization:

The pipeline parameters can be adjusted in the `rnaseq_pipeline.nf` file.  

## Dependencies:

The pipeline requires the following software to be installed:

- FastQC
- Trimmomatic
- HISAT2
- samtools
- featureCounts

