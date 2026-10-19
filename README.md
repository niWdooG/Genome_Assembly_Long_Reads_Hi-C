# De Novo Plant Genome Assembly, Scaffolding & Annotation

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7125249.svg)](https://doi.org/10.5281/zenodo.7125249)
[![GitHub Pages](https://img.shields.io/badge/Live-Interactive_Tutorial-2ea44f?logo=github)](https://niwdoog.github.io/Genome_Assembly_Long_Reads_Hi-C/)
[![Visitors](https://komarev.com/ghpvc/?username=niWdooG-Genome-Assembly&label=Visitors&color=0e75b6&style=flat)](https://github.com/niWdooG/Genome_Assembly_Long_Reads_Hi-C)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> 📖 **Live Interactive Protocol & Tutorial:**  
> Access the complete walkthrough with rendered visual reports, command-line arguments, and code blocks at:  
> **[https://niwdoog.github.io/Genome_Assembly_Long_Reads_Hi-C/](https://niwdoog.github.io/Genome_Assembly_Long_Reads_Hi-C/)**

---

## Overview

This protocol covers end-to-end bioinformatic analyses required to perform chromosome-level scaffolding and annotation of a diploid plant genome using long-read sequencing data (PacBio / Oxford Nanopore) complemented by Hi-C chromatin conformation capture.

### Computational Stack

| Stage | Focus Area | Primary Tools |
| :--- | :--- | :--- |
| **I. Data Processing** | Environment Setup & Ingestion | Conda, SRA Toolkit |
| **II. Assembly** | Error Correction & Contig Assembly | NECAT, NextDenovo, NextPolish |
| **III. Scaffolding** | Chromosome-Level Integration | Hi-C Scaffolding Pipelines |
| **IV. Annotation** | Repeats, Structure & Function | RepeatModeler, RepeatMasker |
| **V. Assessment** | Completeness, Contiguity & Synteny | Qualimap, QUAST, BUSCO, IGV, Circos |

---

## Table of Contents

- **[I] Preface**
  - In a nutshell
  - Learning outcomes
  - Keywords & Metadata
- **[II] Software & Sequencing Data**
  - Architecture & specs of the compute server
  - Conda environment configuration
  - Package installation & standalone binaries
  - Downloading raw sequence data
- **[III] Genome Assembly**
  - Step 1: Long-read assembly via NECAT
  - Step 2: NextDenovo assembly alternative
  - Step 3: Decontamination & organellar filtering
  - Step 4: Iterative base polishing (NextPolish)
  - Step 5: Hi-C scaffolding to pseudomolecules
- **[IV] Genome Annotation**
  - Step 1: *De novo* repeat identification & masking (RepeatModeler & RepeatMasker)
  - Step 2: Structural gene prediction
  - Step 3: Functional annotation & gene ontology
- **[V] Quality Assessment & Visualisation**
  - Step 1: Mapping metrics via Qualimap
  - Step 2: Assembly contiguity via QUAST
  - Step 3: *k*-mer distribution & genome profiling
  - Step 4: Benchmarking completeness via BUSCO
  - Step 5: Read alignment inspection in IGV
  - Step 6: Macro-synteny evaluation
  - Step 7: Whole-genome visualization via Circos
- **Acknowledgements & Citation**

---

## Citation

If you use or adapt this protocol in your academic work, please cite the Zenodo archive:

```bibtex
@manual{baiakhmetov_genome_assembly_2022,
  author       = {Baiakhmetov, Evgenii},
  title        = {Genome Assembly using Long Reads and Hi-C},
  year         = {2022},
  publisher    = {Zenodo},
  version      = {v1.0.0},
  doi          = {10.5281/zenodo.7125249},
  url          = {[https://doi.org/10.5281/zenodo.7125249](https://doi.org/10.5281/zenodo.7125249)}
}
