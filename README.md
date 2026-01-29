# NGS, Omics & Viral Genomics Analysis Portfolio

**Author:** Mohana Venkata Phaneendra Reddy Alla  
**GitHub:** https://github.com/mohanaalla-freddy  
**Repository:** `ngs-omics-viral-genomics-portfolio`

## Why this repo (for hiring managers)
This repository is a job-application friendly portfolio that demonstrates applied bioinformatics skills across:
- NGS data QC and preprocessing (FASTQ/BAM/VCF)
- RNA-seq analysis workflows (alignment → quantification → differential expression)
- Viral genomics / mutation profiling
- Reproducible, pipeline-first development (Snakemake/Nextflow-ready)
- Clear reporting and visualization for scientific stakeholders

## Highlights
- **Reproducible environment**: `environment.yml` (Conda)  
- **Example scripts**: `scripts/` (Python + R templates for common genomics tasks)  
- **Workflow templates**: `workflows/` (Snakemake + Nextflow starter pipelines)  
- **Reports & write-ups**: `docs/` (coursework + NGS/omics analysis report)

## Repository Structure
```
.
├── docs/                       # Reports, homework, analysis summaries (PDF/DOCX)
├── scripts/                    # Example Python/R scripts (ready-to-run templates)
├── workflows/
│   ├── snakemake/              # Snakemake starter pipeline (QC → align → counts → DE)
│   └── nextflow/               # Nextflow starter pipeline (skeleton + notes)
├── environment.yml             # Reproducible software environment
├── CITATION.cff                # Citation metadata
├── LICENSE                     # MIT license
└── README.md
```

## Included Reports (docs/)
- `Mohana_NGS_Omics_data_analysis_report.pdf` — consolidated omics/NGS analysis report  
- `Mohana_Homework_1.pdf` … `Mohana_Homework_8.pdf`, `Homework_5.docx`, `Homework_7.pdf` — supporting coursework deliverables

## Quick start (local)
```bash
# 1) Create environment
conda env create -f environment.yml
conda activate bioinformatics-env

# 2) Run example scripts
python scripts/fastq_qc_summary.py --fastq-dir /path/to/fastq --out qc_summary.csv
python scripts/vcf_variant_stats.py --vcf /path/to/sample.vcf.gz --out variants.tsv
python scripts/bam_alignment_stats.py --bam /path/to/sample.bam --out bam_stats.json

# 3) Run Snakemake starter workflow (edit config first)
cd workflows/snakemake
snakemake -n
snakemake --cores 8
```

## Notes on code quality
- Scripts are **documented**, include **argparse**, and are written to be readable and easy to extend.
- Workflow templates are intentionally minimal and designed to show pipeline structure (rules/stages, inputs/outputs, logs).

## Contact
If you’d like to discuss the projects or request additional code samples (e.g., long-read, assembly, SV), open an issue on GitHub or reach out via my profile.
