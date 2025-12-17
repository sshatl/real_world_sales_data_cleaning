
# Real-World Sales Data Cleaning

This project demonstrates an end-to-end data cleaning pipeline using real-world sales data from a small retail business.

The dataset reflects manual data entry and batch-based extraction, resulting in structural issues, missing values, and mixed record types.  
The goal of this project is to audit the data, apply transparent cleaning steps, and produce analysis-ready datasets.

---

## Dataset Overview

- Time period: 2023–2025  
- Primary product category: laptops  
- Additional records: accessories, refunds, miscellaneous operations  
- Currency: UAH (with derived USD values)

Raw data is not included in the repository due to privacy considerations.

---

## Data Cleaning Workflow

The cleaning process follows a clear, step-by-step pipeline:

1. **Initial data audit**  
   - Identification of structural empty rows  
   - Analysis of partially filled records  

2. **Removal of structural artifacts**  
   - Rows introduced by batch-based extraction  

3. **Separation of non-sales operational records**  
   - Accessories, refunds, miscellaneous transactions  

4. **Handling incomplete sales records**  
   - Retained with explicit missing-value flags  

5. **Date standardization**  
   - Conversion to datetime without fabricating values  

6. **Categorical and text normalization**  
   - Standardized manager field  
   - Basic normalization of product descriptions  

7. **Currency feature creation**  
   - Year-based USD conversion while preserving original UAH values  

---


## Output Datasets

- `sales_clean.csv` — cleaned laptop sales data, ready for analysis and feature engineering  
- `other_operations.csv` — non-sales operational records separated for independent analysis  

---

## Notes

- Missing values are handled explicitly using boolean flags.
- No synthetic or fabricated data is introduced.
- The notebook is fully reproducible using **Restart & Run All**.

---

## Next Steps

- Feature engineering from product descriptions  
- Exploratory analysis and visualization  
- Optional modeling or business insights
