# Methods of Advanced Data Engineering Project

This template project provides some structure for your open data project in the MADE module at FAU. This repository contains (a) a data science project that is developed over the course of the semester, and (b) the exercises that are submitted over the course of the semester.

## Data science project overview

My data engineering project has the following topic: 
## The link between health status and net greenhouse gas emissions in the EU: a cross-country analysis.
This project focuses on analyzing the relationship between Healthy Life Years (HLY) and Greenhouse Gas Emissions (GHG) across European Union countries, utilizing data sourced from Eurostat. The aim is to explore how environmental factors, specifically emissions, correlate with public health outcomes represented by healthy life expectancy at birth.

### ETL Pipeline

**Extract:** The data extraction involves pulling structured datasets directly from Eurostat. These datasets provide detailed annual records of HLY and GHG emissions per capita for EU countries. Data extraction is performed using Python's pandas library, performing direct downloading and reading of CSV files.

**Transform:** The transformation stage includes:
- Filtering out unnecessary columns and rows that are not relevant to the analysis, such as specific gender data which is not used.
- Handling missing values, particularly ensuring that data for all countries covers the same time period (2011-2022). This involves adding missing years for countries like Iceland and interpolating values to maintain consistency across the dataset.

**Load:** The final stage involves loading the cleaned and transformed data into a structured SQLite database. This step ensures the data is stored in a format that is easy to access and analyze for future research or operational use.

### Analysis approach

The project employs statistical methods to understand the dynamics between HLY and GHG emissions. It includes (a) visualizing data trends and disparities between countries and (b) applying correlation analysis to quantitatively assess the relationship between public health metrics and environmental impacts.

### Tools and libraries

- **Python**: Used for scripting and handling data operations.
- **Pandas and Numpy**: Libraries used for data manipulation and numerical calculations.
- **Matplotlib and Seaborn**: For data visualization.
- **SQLAlchemy**: To interact with databases.
- **SQLite**: Database used to store and manage processed data.

All project work submissions are placed in the `project` folder.

## Exercises
During the semester I also completed exercises using [Jayvee](https://github.com/jvalue/jayvee). The submissions are places in the `exercises` folder.

### Exercise Badges

![](https://byob.yarr.is/segalanastasiia/made-template/score_ex1) ![](https://byob.yarr.is/segalanastasiia/made-template/score_ex2) ![](https://byob.yarr.is/segalanastasiia/made-template/score_ex3) ![](https://byob.yarr.is/segalanastasiia/made-template/score_ex4) ![](https://byob.yarr.is/segalanastasiia/made-template/score_ex5)
