# GEOG5995M Final Project: Analysing the Interplay Between Economic Activity and Student Migration in England and Wales

## Overview
This repository contains the GEOG5995M Final Project by Yihang Bai, focusing on a detailed geographical analysis of the interplay between economic activity and student migration in England and Wales. The project utilizes a range of geospatial analysis techniques to explore how economic factors influence student migration patterns, providing crucial insights for urban planning and policy formulation.

### Project Significance
The movement of students across regions is a phenomenon with significant implications for urban development, transportation planning, and economic growth. Understanding these migration patterns is essential for creating sustainable and efficient urban environments. This project aims to shed light on the intricate relationship between economic health and student migration, offering a nuanced perspective on how these factors interconnect and vary across different geographical locations.

This research project embarks on an exploratory analysis of the intricate relationship between economic activity status and student migration patterns within England and Wales. The focus is particularly placed on English Lower Tier Local Authorities (LTLAs) as the unit of analysis, offering a detailed and localized perspective on the phenomenon. Utilizing student migration data and local economy activity status data, the project delves into an in-depth analysis of economic indicators and their potential influence on the migration decisions of students. This approach is grounded in the hypothesis that economic status within specific regions will significantly sways the migratory trends among the student population. The investigation employs a robust methodological framework, leveraging Python's data processing capabilities, coupled with geospatial analysis and advanced visualization techniques, to dissect and interpret the intricate patterns that emerge.

### Research Objectives
The key objectives of this project include:

- Investigating the correlation between economic activity and student migration across England and Wales using Ordinary Least Squares (OLS).
- Examining spatial heterogeneity in the relationship between these factors across England and Wales by employing Geographically Weighted Regression (GWR), providing a comprehensive understanding of the spatial dynamics involved.
- Producing data visualisation of statistical analysis results and student migration combined with local economy status, to demonstrate the research findings to the public.

## Repository Contents
This repository is structured to provide a comprehensive overview of the project's methodology and findings:

### Jupyter Notebook (`GEOG5995M_Final_Project_YihangBai.ipynb`)
A detailed Jupyter notebook containing all the code, analysis, visualizations, and narrative explanations. It is divided into several sections, each dedicated to a specific aspect of the research:
1.	Introduction: Provides an overview of the project's objectives and the significance of the study.
2.	Data import and cleaning: Details the process of preparing the datasets for analysis, emphasizing data integrity and accuracy.
3.	Statistical analysis: Discusses the methodologies employed for spatial analysis, including OLS and GWR.
4.	Data Visualization: Showcases a variety of visualizations, such as maps and scatter plots, to aid in interpreting the data.
5.	Conclusion: Summarizes the key findings and their implications for urban planning and policy-making.

### UK boundary data (`England and Wales LTLAs 2022.7z`)
The boundary data for England and Wales were obtained from the UK Data Service. To align with the dataset, the English Lower Tier Local Authorities (LTLA) were specifically chosen as the geographical unit of analysis.
Note: You need to unzip the LTLA shape file to the original folder to run the code in the jupyter notebook.

### Economy activity status data (`Employment.csv`)
The dataset provides estimates from the 2021 Census, categorizing usual residents in England and Wales, aged 16 and over, based on their economic activity status. This classification encompasses three primary categories: those who are economically active and employed, those who are economically active but unemployed, and those who are economically inactive. In this study, the proportion of economically active individuals is utilized as a measure of local economic health. For comparative purposes, the dataset also includes economic activity data from the 2011 Census.

### Student flow data (`ODST01EW_LTLA.csv`)
The dataset employed in this study offers estimates from the 2021 Census regarding usual residents of England and Wales, aged 16 and over, who resided at a different address one year prior to the Census. This previous address was either a student term-time location or a boarding school address within the UK. The data categorizes these individuals based on their relocation from one Lower Tier Local Authority (LTLA) area to another, comparing their location one year before the Census with their current LTLA residence as of Census Day, 21 March 2021.

### Python Environment File (`env.yml`)
A file that creates a coding environment for replicating the analysis, including libraries for data cleaning, geospatial analysis, and visualization. You may need to create the environment by code: ` conda env create -f env.yml`.

## Code Description and Analysis Techniques
The project uses Python as the primary programming language, with an emphasis on libraries like pandas, geopandas, matplotlib, and seaborn for data manipulation and visualization. Key analysis techniques include:
- Ordinary Least Squares (OLS) Regression
- Geographically Weighted Regression (GWR)
Note: You are required to use code 'pip install mgwr' to conduct the GWR analysis in the jupyter notebook.

The analysis uncovers significant correlations and spatial variability between economic factors and student migration patterns, highlighting the influence of economic health on migration decisions.

## Running the Code
To replicate this analysis:
1. Install Python 3.8 and Jupyter Notebook or JupyterLab.
2. Clone the repository to your local machine. Unzip the LTLA shape file to the original folder.
3. Create the coding environment using `conda env create -f env.yml`.
4. Open and run the cells in `GEOG5995m_Final_Project_YihangBai.ipynb` sequentially.

## Contributions and Future Directions
This project is open for contributions and further research. The findings underscore the importance of economic indicators in urban planning, particularly in areas with high student populations. Future research could explore more detailed data or additional factors influencing student migration.
