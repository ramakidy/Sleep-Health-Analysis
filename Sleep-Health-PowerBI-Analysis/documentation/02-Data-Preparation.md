# Data Preparation Process

## Data Source
- **Original File:** `Sleep_health_and_lifestyle_dataset.csv` from Kaggle.
- **Tool:** Microsoft Excel.

## Data Cleaning and Transformation in Excel

### Steps Performed:

1. **Data Loading**
   - Imported CSV into Excel.

2. **Field Renaming**
   - Used Find and Replace to standardize column names.

3. **New Field Creation**
   - **Age Group:** Used nested IF to categorize ages into Young Adult (27-35), Middle Age (36-50), Old Adult (51-59).
   - **Blood Pressure Group:** Nested IF to classify BP based on clinical standards.
   - **BMI Category:** Nested IF to assign BMI categories (Underweight, Normal, Overweight, Obese).

4. **Data Cleaning**
   - Find and Replace to standardize categorical values.

5. **Advanced Operations**
   - VLOOKUP for basic data matching and enrichment.

### Excel Formulas Examples:

#### Age Group
```excel
=IF(Age<=35, "Young Adult", IF(Age<=50, "Middle Age", "Old Adult"))