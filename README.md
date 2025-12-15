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

## Psychometric Scales and Latent Indicators
The core analysis relies on converting observed items into latent factors. The dataset contains item-level data derived from validated instruments.   

### The Nomophobia Construct (MR1) 

Nomophobia1: Anxiety regarding forgetting the smartphone.

Nomophobia2: Discomfort when the device is out of reach.

Nomophobia3: Worry regarding battery/signal loss (technological anxiety).

Nomophobia4: Anxiety regarding unchecked notifications (informational anxiety).

Nomophobia5: Discomfort regarding communication latency (social anxiety).

## The Sleep Quality Construct (MR2) 

Daytime_sleepiness: Frequency of struggling to stay awake during academic tasks.

Night_sleep_hours: Self-reported average sleep duration.

Sleep_disturbance: Frequency of nocturnal awakenings.

Subjective_sleep_quality: A global self-rating of sleep hygiene.

Sleep_onset_latency: The time taken to transition from wakefulness to sleep.

### The Study Distraction Construct (MR3) 
Studytime_phone_check_frequency: The frequency of interruptions during study sessions.

Studytime_notification_distraction: The subjective impact of push notifications.

Independent_learning_hours: A reverse-coded proxy for focus; lower hours often correlate with higher distraction.

NonAcademic_screen_time: Time spent on entertainment/social media, hypothesized to compete with study time.

### Outcome Variables (Academic Performance)
GPA: The cumulative Grade Point Average, a continuous variable serving as the primary outcome variable in the path analysis model.   

ClassGPA: A categorical derivation of GPA, used in the Exploratory Data Analysis phase for logistic regression checks.   


