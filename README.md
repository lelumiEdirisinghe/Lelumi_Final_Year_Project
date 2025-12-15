# Determinants of Academic Performance

## Repository Usage and Reproduction Guide
This repository is structured to facilitate full reproduction of the analysis.

### System Requirements
Software: R (version 4.0 or higher) and RStudio.

Key Libraries: The analysis requires the installation of the following packages:

```{r,warning=FALSE}
install.packages(c("lavaan", "psych", "MVN", "boot", "tidyverse", 
                   "readxl", "summarytools", "corrplot", "car", 
                   "pROC", "sjmisc", "broom", "kableExtra"))
```
## Execution Instructions

Please make sure finalDataset.xlsx is placed in the project root directory, the Final. Rmd script is configured to look for this file in the working directory.

The script  will automatically perform the cleaning, EFA, and SEM, and generate the summary tables and plots.
