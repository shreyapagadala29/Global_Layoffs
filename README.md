# Global_Layoffs
# Global Layoffs EDA Project

## Introduction
The layoffs dataset offers detailed information on layoffs that have occurred in a number of companies in various locations. It contains the names of the companies, their locations, the number of laid-off employees, and the dates of the layoffs. The primary purpose of analyzing this dataset is to identify trends and evaluate the impact on different regions and industries. This analysis makes it easier to grasp the overall number of layoffs by nation and area, pinpoint the organizations that have had the most layoffs, and see how layoffs have changed over time.

## Problem Statement
This project aims to perform an exploratory data analysis (EDA) of layoffs in various locations, industries, and stages of the organization. The goals are to spot trends, show how layoffs have changed over time, and draw attention to the main causes of layoffs. This study will shed light on the most impacted industries and locations, the timing of layoffs, and the traits of the businesses that are being laid off at the greatest rate.

## Data Overview
The layoffs dataset contains information about layoffs across various companies and locations. Each record in the dataset includes the following columns:

- **Company**: The name of the company where layoffs occurred.
- **Location**: The geographical location of the company.
- **Industry**: The industry to which the company belongs.
- **Total Laid Off**: The number of employees laid off from the company.
- **Percentage Laid Off**: The percentage of the company's workforce that was laid off.
- **Date**: The date on which the layoffs were reported.
- **Stage**: The funding or operational stage of the company at the time of layoffs.
- **Country**: The country where the layoffs occurred (e.g., Australia, United States).
- **Funds Raised (Millions)**: The total amount of funds raised by the company in millions.

## Snapshot of Layoffs Dataset
A snapshot of the dataset reveals critical details necessary for analysis, including company names, locations, industries, and the magnitude of layoffs.

<img width="1440" alt="Screenshot 2025-01-09 at 2 00 41 PM" src="https://github.com/user-attachments/assets/1f487d49-387b-48f2-a052-68505b416477" />


## Data Cleaning
There were many cleaning stages performed to prepare the layoffs dataset for exploratory data analysis:

1. Missing values in the `Percentage Laid Off` column were resolved.
2. The `Date` column was transformed into the correct date format.
3. Inaccurate or unclear entries in columns such as `Location`, `Industry`, `Stage`, and `Country` were standardized.
4. Duplicates in the dataset were identified and eliminated.
5. Numerical data, including `Total Laid Off` and `Funds Raised (Millions)`, were inspected for consistency and adjusted as needed.

## Snapshots Cleaning Data of in MySQL
<img width="1440" alt="Screenshot 2025-01-09 at 1 58 23 PM" src="https://github.com/user-attachments/assets/2205f148-d478-40be-a3a6-eb4dffdc8b99" />


## Data Exploration
Key findings from the exploratory data analysis include:

- **Impact of COVID-19**: Many companies experienced increased layoffs due to the COVID-19 pandemic by early 2023.
- **Industries with the Most Layoffs**: Consumer & retail industries were heavily impacted, likely due to office closures during the pandemic.
- **Countries with the Most Layoffs**: The United States recorded the highest number of layoffs, with 256,420 layoffs.
- **Locations with the Most Layoffs**: The SF Bay Area had the highest number of layoffs, totaling 125,551, likely due to the region's high number of COVID-19 cases.

### Progression of Layoffs by Year
- Used rolling sums in MySQL and breakdowns by year to understand the progression of layoffs.
- Ranked companies by layoffs per year using Common Table Expressions (CTEs) to identify the top 5 companies.

## Key Insights
### Companies with the Highest Layoffs:
- **Amazon**: 18,150 layoffs
- **Google**: 12,000 layoffs
- **Meta**: 11,000 layoffs
- **Salesforce**: 10,090 layoffs
- **Microsoft**: 10,000 layoffs

### Location with the Highest Layoffs:
- **Seattle**: Amazon accounted for 54,430 layoffs.

### Progression of Layoffs:
- **March 2020**: Rolling total of 9,628 layoffs
- **December 2020**: Rolling total of 80,998 layoffs
- **January 2021**: Rolling total of 87,811 layoffs
- **December 2021**: Rolling total of 96,821 layoffs (2021 was a relatively better year compared to others)
- **January 2022**: Rolling total of 97,331 layoffs
- **December 2022**: Rolling total of 257,143 layoffs (2022 was the worst year for layoffs)
- **2023**: Data is incomplete as it only includes early 2023.

### Variance in Layoffs and Fundraising:
There is a higher variance in both the number of layoffs and funds raised in the 1% layoffs than the 0% layoffs.

### Top Companies with the Most Layoffs Each Year:
- **2020**: Uber with 30,100 layoffs
- **2021**: ByteDance with 7,200 layoffs
- **2022**: Amazon with 20,300 layoffs
- **2023**: Google with 12,000 layoffs

### Suggestion Strategy:
1. Provide specialized assistance programs for industries such as retail, transportation, and real estate, including financial aid packages, retraining programs, and staff retention incentives.
2. Implement early warning systems and trend tracking to anticipate and address possible layoff surges, allowing for proactive measures to lessen the effects.
