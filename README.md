# ASBQ_Survey_Code

Sleep Survey Analysis – Fall 2025
Overview

This R Markdown script analyzes sleep behaviors of student-athletes across different seasons (Pre-Season and Post-Season).

The script:

Loads survey data (.csv)

Cleans and transforms variables

Converts Likert-scale responses to factors and numeric values

Creates bar plots of survey responses by sport and season

Performs statistical tests for each survey item:

Mann-Whitney U tests (numeric Likert scores)

Chi-square tests (categorical counts)

Analysis Approach

Survey data is cleaned with dplyr and janitor

Likert responses converted to numeric for Mann-Whitney testing

Counts summarized and plotted with ggplot2 by sport and season

Seasons ordered: Pre-Season → Mid-Season

R Packages Used

ggplot2

dplyr

janitor

Required Input File

.csv

Must include columns:

Date

Sport

Class/Status

Sleep survey responses (Likert items)

Update the file path in the script before running:

input_path <- file.path("YOUR/DATA/DIRECTORY", "example_file.csv")
Output

Bar plots of each survey variable by season and sport

Mann-Whitney U and Chi-square test results for each survey variable

Knitted HTML report showing plots and printed test results
