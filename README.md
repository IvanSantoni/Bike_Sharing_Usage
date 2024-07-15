# Bike-Sharing Usage Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)

### Project Overview

This data analysis project aims to provide insight into the usage performance of a bike-sharing company over one year. By analyzing various aspects of the usage data, we seek to identify trends, make data driven reccomandation and gain deeper understanding of the company's performance.

### Data Sources

Usage Data: The datasets used for this analysis are 'usage.csv' files, containing detailed information about each use made for every month by the company's customer.

### Tools

- Excel: Data Cleaning
    -  [Download here](https://divvy-tripdata.s3.amazonaws.com/index.html)
- SQL Server: Data Analysis
- Tableau - Creating reports

### Data Cleaning

In the initial data preparation phase, we perform the following tasks:
1. Data loading and inspection;
2. Handling missing values;
3. Data cleaning and formatting.

### Exploratory Data Analysis

EDA involved exploring the sales data to answer key question, such as:

- What is the average time by users?
- Which product are the most used?
- What are the peaks of usage periods?

### Data Analysis

Include some interesting code/features worked with

```sql
SELECT avg(ride_length) as avg_time
FROM 2024_rides
GROUP BY member_casual;
```
```sql
LOAD DATA INFILE
'C:\\ProgramData\\MySQL\\MySQL Server 8.0\\Uploads\\[file_name].csv'
INTO TABLE 2024_rides
FIELDS TERMINATED BY ','
IGNORE 1 LINES;
```

### Results

The analysis results are summarized as follows:
1. The company usage increase from April to September when the wheater is mild.
2. The usage drops during the cold months.
3. Casuals users use bikes for more time in average then members.
4. The classic bike is the best-performing product in terms of usage, and the docked bike is the last one.

### Recommendations

Based on the analysis, we recommend the following actions:
- Focus on expanding and promoting classic bike usage.
- Implement a discount strategy during the cold months, to promote bike usage.
- Find a strategy to target the members usage effectively.

### Limitations

I had to remove the distance covered by each use of everybike because they would have affected the accuracy on my conclusion from the analysis.


### References

1. MySQL
2. [Stack Overflow](https://stackoverflow.com/)




