# 🧬 FASTQ to Differential Expression Pipeline (Kallisto + DESeq2)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/XGhoster1/fastq-to-DE/blob/main/notebooks/kallisto_pipeline.ipynb)

This repository contains a complete lightweight RNA-seq pipeline that takes raw FASTQ files to differential gene expression results using:

- **Kallisto** for transcript quantification (alignment-free, fast)
- **DESeq2** for differential expression in R
- **Google Colab** for cloud-based reproducibility

---

## 📂 Project Structure

fastq-to-DE/
├── data/
│ ├── fastq/ # Raw FASTQ files
│ ├── reference/ # Transcriptome FASTA + index
│ └── kallisto_output/ # Kallisto quantification outputs
├── results/ # DE results and visualizations
├── scripts/ # Shell scripts (optional)
├── notebooks/
│ └── kallisto_pipeline.ipynb # Core notebook to run on Colab
├── environment.yml # Conda environment for local setup
└── README.md


---

## 🚀 Usage

### ▶️ Run on Google Colab

Click the badge at the top or [open this notebook](https://colab.research.google.com/github/XGhoster1/fastq-to-DE/blob/main/notebooks/kallisto_pipeline.ipynb) to launch in Colab.

This will:
1. Install `kallisto`
2. Download example FASTQ file (SRR1215996)
3. Download Ensembl GRCh38 cDNA FASTA
4. Build transcriptome index
5. Run `kallisto quant` (single-end example)

---

## 🧠 Coming Soon

- 🧬 `tximport` + `DESeq2` differential expression
- 📊 Volcano plot, PCA, and heatmaps
- 🧰 Modular shell scripts for local/cluster execution

---

## 🙌 Author

Created by [@XGhoster1](https://github.com/XGhoster1) as a portfolio project. Contributions, feedback, and forks welcome!
