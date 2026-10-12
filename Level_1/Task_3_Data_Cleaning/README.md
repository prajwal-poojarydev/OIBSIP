# Data Cleaning and Preprocessing

**Internship:** Oasis Infobyte – AICTE Data Analytics Internship  
**Task:** Level 1 – Task 3  
**Author:** Prajwal Poojary

## Project Overview

This project focuses on cleaning and preprocessing a deliberately messy customer dataset using Python, pandas, NumPy, and Jupyter Notebook. The goal was to improve data consistency, identify quality issues, handle missing values, standardise formats, and export a cleaned dataset for further analysis.

## Dataset

- **Source:** [Datanemics – Dirty Customers Dataset](https://datanemics.com/datasets/dirty-customers/)
- **Original records:** 1,000
- **Columns:** 8
- **Fields:** Customer ID, full name, email, signup date, country, spending, customer segment, and active status.

## Tools and Technologies

- Python
- pandas
- NumPy
- Jupyter Notebook

## Data Cleaning Process

1. **Initial inspection:** Examined the dataset structure, data types, missing values, duplicate records, inconsistent categories, and unusual spending values.
2. **Duplicate removal:** Removed exact duplicate records, including duplicates revealed after standardising values. The dataset was reduced from 1,000 to 957 rows.
3. **Missing-value handling:** Converted placeholders such as `none`, `-`, and `-999` into proper missing values where applicable.
4. **Spending standardisation:** Removed currency labels, currency symbols, and thousands separators before converting spending values to numeric format.
5. **Outlier treatment:** Used the interquartile range (IQR) method to identify unusually high spending values. Values above the upper IQR boundary of approximately 1,381.03 were capped rather than deleting entire customer records.
6. **Median imputation:** Filled missing spending values using the median of the cleaned, outlier-capped spending values (252.99).
7. **Category standardisation:** Unified country names and customer segment labels.
8. **Name and email standardisation:** Trimmed whitespace, standardised name casing, and converted emails to lowercase. Clearly identifiable email addresses wrapped in angle brackets were extracted. Remaining malformed email formats were marked as missing rather than guessed.
9. **Date processing:** Converted signup dates to datetime format. Unknown or unparseable dates were retained as missing.
10. **Data type correction:** Converted customer IDs and text fields to string types, spending to numeric, signup dates to datetime, and active status to Boolean.

## Before-and-After Summary

| Metric | Before cleaning | After cleaning |
|---|---:|---:|
| Rows | 1,000 | 957 |
| Total missing values | 100 | 122 |
| Exact duplicate rows | 1 | 0 |
| Key columns with correct target data types | 0 | 4 |

The missing-value count increased because placeholder values were converted into proper missing values and malformed email addresses were marked as missing. These changes make the remaining data-quality issues explicit rather than hiding them.

## Output Files

- `PrajwalPoojary_Task3.ipynb` — Notebook containing the cleaning workflow and analysis.
- `PrajwalPoojary_Task3_Cleaned.csv` — Cleaned customer dataset.

## Limitations and Assumptions

- IQR-based capping is a statistical treatment and does not prove that every extreme value was erroneous.
- Missing email addresses and signup dates were not invented or imputed.
- Email validation checks basic formatting only; it does not confirm that an address exists.
- Ambiguous date strings were parsed using pandas' mixed-format parsing behaviour and may require source-level verification.
- The dataset was checked for exact duplicate rows. Repeated customer IDs with differing records were not automatically deleted.

## Conclusion

The project demonstrates a structured data-cleaning workflow, including data quality inspection, duplicate removal, missing-value handling, standardisation, outlier treatment, data type correction, and validation of the exported CSV. The cleaned dataset is ready for further analysis, subject to the documented limitations.