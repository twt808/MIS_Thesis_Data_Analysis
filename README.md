# Data Analysis Pipeline for the Master’s Thesis

## Project Title

**Conceptualising Technology Threat Avoidance Theory (TTAT) to Examine Cognitive Risks of Generative AI in Higher Education**

**Author:** Tshering Wangchuk  
**Institution:** University of Canberra  
**Degree:** Master of Information Science (Research)  
**Year:** 2026

## Overview

This repository contains the R Markdown analysis pipeline and the corresponding knitted HTML output used for the thesis titled *Conceptualising Technology Threat Avoidance Theory (TTAT) to Examine Cognitive Risks of Generative AI in Higher Education*.

The files are provided to improve the transparency, traceability, and reproducibility of the data-preparation and statistical-analysis procedures reported in Chapters 4 and 5 of the thesis. The analysis was conducted in RStudio using a single R Markdown workflow.

## Repository files

| File | Description |
|---|---|
| [`Data_Analysis_Final_Revised.Rmd`](./Data_Analysis_Final_Revised.Rmd) | The executable R Markdown source file containing the R code, analytical steps, comments, tables, and figures used in the study. |
| [`Data_Analysis_Final_Revised.html`](./Data_Analysis_Final_Revised.html) | The knitted HTML output generated from the R Markdown file. It provides a viewable record of the code, outputs, tables, figures, model results, and diagnostics produced during the analysis. |

> Update the filenames in this README if the files in the repository use different names.

## Purpose of the analysis

The analysis examines how university students perceive, avoid, and cope with cognitive risks associated with the use of Generative Artificial Intelligence in higher education. It applies an extended Technology Threat Avoidance Theory framework and examines:

- students’ perceived cognitive risks associated with GenAI use;
- demographic and experiential predictors of Perceived Threat;
- threat-appraisal, coping-appraisal, Avoidance Motivation, and coping-behaviour relationships; and
- students’ expectations regarding institutional measures for safer and more responsible GenAI use.

## Analysis workflow

The R Markdown pipeline documents the main stages of the analysis:

1. Importing the two REDCap survey exports.
2. Filtering records associated with suspected automated responses.
3. Aligning and merging the valid survey records.
4. Removing REDCap administrative fields.
5. Converting blank responses to missing values.
6. Distinguishing required and optional survey fields.
7. Assessing response completeness and data quality.
8. Checking coded values, duplicate records, and straightlining patterns.
9. Retaining complete records for the final analytical sample.
10. Recoding demographic and experiential variables.
11. Reverse-scoring Perceived Costs where required.
12. Computing the TTAT construct composite scores.
13. Producing demographic and construct-level descriptive statistics.
14. Generating tables, histograms, boxplots, correlation visualisations, and scatterplots.
15. Conducting the linear-regression models used for hypothesis testing.
16. Assessing relevant regression assumptions and model diagnostics.
17. Extracting supplementary open-ended responses for descriptive review.

The final analytical sample used in the thesis contained **139 complete responses**.

## Analytical approach

The pipeline includes:

- frequency and percentage summaries;
- means, standard deviations, medians, and ranges;
- composite-score computation using item-level means;
- descriptive visualisations;
- correlation analysis;
- ordered-score regression models;
- binary-group and planned-contrast models;
- simple linear regression;
- multiple linear regression; and
- regression diagnostics.

Open-ended survey responses were treated as supplementary descriptive material and were not analysed as an independent qualitative dataset.

## Software requirements

The analysis was developed in **RStudio** using **R Markdown**.

To inspect the source code, open the `.Rmd` file in RStudio or another text editor. To reproduce the analysis, an authorised user will need:

- a current installation of R;
- RStudio or another environment capable of rendering R Markdown;
- the R packages loaded near the beginning of the `.Rmd` file; and
- authorised access to the original REDCap CSV exports.

Missing packages can be installed in R using:

```r
install.packages("package_name")
```

The exact packages required should be identified from the library-loading section at the beginning of the R Markdown file.

## Reproducing the analysis

The repository does **not** include the raw survey data. Therefore, the full analysis cannot be rerun from the public repository alone.

An authorised researcher with access to the original data can reproduce the workflow by:

1. Downloading or cloning this repository.
2. Opening `Data_Analysis_Final_Revised.Rmd` in RStudio.
3. Installing any required R packages.
4. Placing the authorised REDCap CSV exports in an appropriate local folder.
5. Updating the input file paths in the R Markdown file.
6. Running the code sequentially or knitting the document to HTML.

The cleaned analytical dataset is recreated within the R Markdown workflow rather than being stored as a separate public data file.

## Data availability and confidentiality

The raw survey data are not publicly available because they were collected from human participants under University of Canberra ethics approval and are subject to research-data management, confidentiality, and secure-storage requirements.

The main survey was designed to collect anonymous responses. Optional contact information used for the prize draw or distribution of the research summary was collected and stored separately from the survey responses.

The exclusion of the raw data means that this repository supports transparency and verification of the analytical procedures and reported outputs, but not unrestricted reproduction by users who do not have authorised data access.

## Relationship to the thesis

The R Markdown file documents the data preparation and analysis procedures described in **Chapter 4: Research Design and Methodology**.

The knitted HTML file contains the analytical outputs supporting **Chapter 5: Data Analysis and Results**.

The repository is referenced in **Appendix E: Data Analysis Pipeline (R Markdown and Output File)** of the thesis.

## Viewing the HTML output

The HTML file is a static record of the knitted R Markdown analysis. Depending on the browser and GitHub settings, GitHub may display the file source or prompt the user to download it rather than render it as a webpage.


## Citation

When referring to the analytical materials in this repository, the following format may be used:

> Wangchuk, T. (2026). *Data analysis pipeline for Conceptualising Technology Threat Avoidance Theory (TTAT) to Examine Cognitive Risks of Generative AI in Higher Education* [R Markdown and HTML files]. GitHub. `[Insert repository URL]`

## Ethics

The study received approval from the University of Canberra Human Research Ethics Committee under **Project ID 76147**.

## Contact

**Tshering Wangchuk**  
Master of Information Science (Research)  
University of Canberra  

Contact details may be added here if a public research email address is available.

## Licence

No licence has been specified in this draft. Add an appropriate software or research-output licence before public reuse or redistribution is permitted.
