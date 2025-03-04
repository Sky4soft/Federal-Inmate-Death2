# Federal Inmate Deaths Analysis

## Background
This repository contains data obtained by the [Data Liberation Project](https://www.data-liberation-project.org/), via a [Freedom of Information Act request](https://www.data-liberation-project.org/requests/ssvf-satisfaction-surveys/) to the US Department of Veterans Affairs (VA) and pre-processed by the Data Liberation Project. The goal of this project is to explore patterns and trends in inmate deaths within the federal prison system, analyzing factors such as **death categories, demographic distributions, and geographic trends**.

## FOIA Records
The records provided by the VA by the Data Liberation Project can be viewed [HERE](https://docs.google.com/spreadsheets/d/1VyoVX2PEQXSaUJ9dNTvJ36HNBE5tGLcy/edit?gid=1808560422#gid=1808560422).

## Code
This repository contains one Malloy code file:
- [`prison1.malloynb`](prison1.malloynb), which performs the analysis of the data provided by the Data Liberation Project.

## Motivation
Underatanding the causes and patterns of inmate deaths is essential for:
- Identifying preventable causes,
- Highlighting public health concerns in the prison system.
- Supporting transparency and accountability within federal institutions.
- Providing insights for policymakers and advocacy groups focused on prison reform.

## Summary of Findings
After analyzing the dataset, several key insights emerged:
- **Cardiac-related deaths** are the most common cause.
- The highest number of deaths occurred during the **COVID-19 pandemic (2020)**.
- Specific institutions consistently report higher death counts.
- The most common death categories are **Cardiac, Cancer, Pulmonary, Liver**, and **Unknown**.
- **Demographic patterns** reveal disparities across sex and race groups.

## Data Sources  
The dataset includes records of federal inmate deaths, providing details such as:  
- **Date of Death (DOD)**  
- **Cause of Death (ICD-10 Codes)**  
- **Demographics (Race, Sex, Age, Location)**  
- **Prison Facility (Institution ID, State, County)**  

## Datasets
- prison.csv: Primary dataset of inmate deaths.
- categories.csv: Category definitions for causes of death.
- Additional support files, such as locationplace.csv and wheretogo.csv are included for geospatial analysis.

## Data Cleaning Steps
To ensure reliable analysis, the following cleaning steps were performed:
- Removed records with incomplete or ambiguous dates.
- Standardized **ICD-10** codes to group causes of death.
- Cleaned and unified inconsistent **city, state**, and **institution ID** fields.
- Filled missing categories with `"Unknown"` to maintain data consistency.
- Filtered out invalid entries or duplicates in the dataset.

## How to Open a Shared GitHub File and Run Malloy Code
To explore the data and run the analyses:

Click on the (https://github.com/Sky4soft/Federal-Inmate-Death2) provided to access the shared repository or file. 

Once on Github, click Shift + period this will load the web editor. Then install the malloy extension. See images below for reference:

| **Step**   | **Image Preview** |
|--------|-----------|
| `Step 1 - Press allow` | <img src="./Images/step1.png" width="50%"> |
| `Step 2 - Click the Blocks, search for Malloy, install` | <img src="./Images/step2.png" width="50%"> |
| `Step 3 - Click Trust` | <img src="./Images/step3.png" width="50%"> |
| `Step 4 - Click a .malloynb file` | <img src="./Images/step4.png" width="50%"> |
| `Step 5 - Press Run` | <img src="./Images/step5.png" width="50%"> |

## Key Questions Explored  
- What are the most common causes of death in federal prisons?  
- Are certain causes of death more prevalent in specific locations or institutions?  
- How have inmate death rates changed over time?  
- Are there any observable patterns across demographic groups?  

## Visualizations & Analysis  
This project leverages **Malloy** for querying and analyzing the data. Various visualizations, including **bar charts, line graphs, and scatter plots**, are used to enhance data interpretation.  

This data shows the yearly trends in deaths from Cancer, Liver, Pulmonary, and Unknown causes across different cities and countries.

<img src="./Images/Trend.png">

This data shows the annual distribution of deaths for Cancer, Pulmonary, and Liver categories, and compares these deaths as a percentage of all deaths over the years.

<img src="./Images/Deathdata.png">
<img src="./Images/Death.png">

This data shows that cardiac-related deaths are the highest among all categories.

<img src="./Images/Numberdate.png">
<img src="./Images/Number.png">

This graph shows that the most common causes of death for male inmates since 2005, broken down by race.

<img src="./Images/Race.png">

This graph shows the total deaths for each death category (e.g., Cancer, Cardiac) across all genders.

<img src="./Images/Register.png">

## Licensing
The files provided directly via FOIA (see listing above) are, as government documents, now in the public domain. All other data files have been generated by Julie Moore for Gonzaga University Graduate School of Business as part of the MSBA-622-01 Data Science for Business (Spring 2025) course and are available under Creative Commons’ [CC BY-SA 4.0 license terms](https://creativecommons.org/licenses/by-sa/4.0/). This repository’s code is available under the [MIT License terms](https://opensource.org/license/mit/). 
