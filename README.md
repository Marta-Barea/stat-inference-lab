[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![R](https://img.shields.io/badge/R-Statistical_Inference-276DC3?logo=r&logoColor=white)](https://www.r-project.org/)
[![R Markdown](https://img.shields.io/badge/R%20Markdown-Reports-0B4F6C?logo=rstudioide&logoColor=white)](https://rmarkdown.rstudio.com/)
[![PEC1 PDF](https://img.shields.io/badge/PEC1-PDF-1b5e20)](reports/pec1-probability-distributions.pdf)
[![PEC2 PDF](https://img.shields.io/badge/PEC2-PDF-1b5e20)](reports/pec2-statistical-modeling-and-estimation.pdf)
[![PEC3 PDF](https://img.shields.io/badge/PEC3-PDF-1b5e20)](reports/pec3-hypotesis-testing-and-inference.pdf)

# Statistical Inference Lab

## Overview

This repository contains a reproducible R-based coursework workflow for statistical inference in biological and biomedical contexts. The material is organized as a sequence of continuous assessment reports written in R Markdown and rendered to PDF, combining theoretical development, mathematical derivations, statistical modeling, and computational analysis in R.

The current analytical scope covers:

- probability models and discrete random variables;
- likelihood-based estimation and method of moments;
- confidence intervals and resampling ideas;
- parametric and non-parametric hypothesis testing;
- applied inferential analysis for quantitative and categorical biomedical data;
- reproducible reporting through R Markdown, LaTeX, and PDF output.

## Repository Components

### Statistical reports

The core of the repository is a set of three assessment reports corresponding to different blocks of the course.

- reports/pec1-probability-distributions.Rmd: first report focused on probability distributions and introductory probabilistic modeling.
- reports/pec1-probability-distributions.pdf: rendered PDF for PEC1.
- reports/pec2-statistical-modeling-and-estimation.Rmd: second report focused on statistical modeling, estimation, likelihood, and simulation-based analysis.
- reports/pec2-statistical-modeling-and-estimation.pdf: rendered PDF for PEC2.
- reports/pec3-hypotesis-testing-and-inference.Rmd: third report focused on hypothesis testing and inferential decision-making.
- reports/pec3-hypotesis-testing-and-inference.pdf: rendered PDF for PEC3.

### Report support files

The reports share LaTeX customization assets and visual resources used during document preparation.

- reports/preamble.tex: LaTeX header customizations used by the PDF reports.
- assets/images/: supporting figures and institutional image assets.

### Course materials

The repository also includes the original statement for the third assessment.

- Enunciado_UOC-MU-IE-2025-26-S2-PEC3-2.pdf: source brief for PEC3.

## Project Structure

```text
.
├── assets/
│   └── images/                  # Supporting figures and logo assets
├── reports/
│   ├── pec1-probability-distributions.Rmd
│   ├── pec1-probability-distributions.pdf
│   ├── pec2-statistical-modeling-and-estimation.Rmd
│   ├── pec2-statistical-modeling-and-estimation.pdf
│   ├── pec3-hypotesis-testing-and-inference.Rmd
│   ├── pec3-hypotesis-testing-and-inference.pdf
│   └── preamble.tex
├── Enunciado_UOC-MU-IE-2025-26-S2-PEC3-2.pdf
├── LICENSE
└── README.md
```

## Analytical Scope

Across the three reports, the repository addresses the following statistical topics:

- construction and validation of probability mass functions;
- expectation, variance, and probability calculations for discrete models;
- likelihood functions, maximum likelihood estimation, and method of moments;
- simulation for estimator assessment and sampling behavior;
- confidence interval construction and interpretation;
- chi-squared tests, t tests, Wilcoxon tests, ANOVA, and post hoc comparisons;
- assumption checking and the choice between parametric and non-parametric procedures.

## Main Outputs

The main outputs of the repository are the rendered assessment reports:

- reports/pec1-probability-distributions.pdf
- reports/pec2-statistical-modeling-and-estimation.pdf
- reports/pec3-hypotesis-testing-and-inference.pdf

Each PDF corresponds to a complete, reproducible R Markdown analysis that can also be exported to Word or HTML through the YAML configuration in the source document.

## Requirements

The project is implemented in R and relies primarily on the R Markdown toolchain.

Core requirements:

- R
- rmarkdown
- knitr
- a LaTeX engine compatible with the report configuration

Depending on the specific report, additional statistical or visualization packages may be required by the code chunks used in the analyses.

## Setup

Clone the repository and open it in your preferred R environment.

```bash
git clone git@github.com:Marta-Barea/stat-inference-lab.git
cd stat-inference-lab
```

Example package installation in R:

```r
install.packages(c("rmarkdown", "knitr"))
```

If your local R setup does not yet support PDF generation, install a LaTeX distribution such as TinyTeX.

## Reproducible Workflow

### 1. Render PEC1

```bash
Rscript -e "rmarkdown::render('reports/pec1-probability-distributions.Rmd', output_format = 'pdf_document')"
```

### 2. Render PEC2

```bash
Rscript -e "rmarkdown::render('reports/pec2-statistical-modeling-and-estimation.Rmd', output_format = 'pdf_document')"
```

### 3. Render PEC3

```bash
Rscript -e "rmarkdown::render('reports/pec3-hypotesis-testing-and-inference.Rmd', output_format = 'pdf_document')"
```

The rendered PDFs are written to the reports directory.

## Academic Context

These assignments were developed within the continuous assessment framework of the Interuniversity Master's Degree in Bioinformatics and Biostatistics offered by the Universitat Oberta de Catalunya and the Universitat de Barcelona.

## Access

- PEC1 report: [reports/pec1-probability-distributions.pdf](reports/pec1-probability-distributions.pdf)
- PEC2 report: [reports/pec2-statistical-modeling-and-estimation.pdf](reports/pec2-statistical-modeling-and-estimation.pdf)
- PEC3 report: [reports/pec3-hypotesis-testing-and-inference.pdf](reports/pec3-hypotesis-testing-and-inference.pdf)

## Author

Marta Barea Sepúlveda  
Interuniversity Master's Degree in Bioinformatics and Biostatistics  
Universitat Oberta de Catalunya - Universitat de Barcelona

## License

This project is distributed under the GNU General Public License v3.0. See the LICENSE file for the full license text.
