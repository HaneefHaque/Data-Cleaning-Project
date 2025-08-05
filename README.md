# Data Cleaning Project

### Project Overview

This data cleaning project is on a real-world dataset tracking global layoffs, which included inconsistencies, duplicates, and null values.
The goal was to clean the data so that it could be used for reliable analysis, reporting trends in layoffs by industry, company, country, and time.

### Data Sources

World Layoff Data: The primary dataset used for this project is the "layoffs.csv" file.

### Process

- Removed duplicates using ROW_NUMBER() OVER(...) and SQL DELETE

- Cleaned and standardised text values with TRIM(), LIKE, and UPDATE

- Converted string-based date formats into proper SQL DATE type

- Handled missing values, e.g., through conditional JOINs to infer missing industry entries

- Validated and filtered unusable rows to ensure data integrity

### Result

- Produced a cleaned dataset that could be confidently used for trend analysis and reporting.

### Limitations

- Despite cleaning, some rows still contain null or missing values (e.g., for total_laid_off or industry)
Could be further analysed by cross-referencing external datasets.
