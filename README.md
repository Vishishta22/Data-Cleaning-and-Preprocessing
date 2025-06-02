#  Customer Personality Analysis - Task 1: Data Cleaning

This project focuses on cleaning and preparing the dataset `marketing_campaign.csv`, which contains demographic and purchasing behavior data of customers. The cleaned data will serve as the foundation for future tasks such as exploratory data analysis, segmentation, and predictive modeling.

---

##  Objective

To clean the raw dataset by:
- Handling missing values
- Removing duplicates
- Standardizing text values
- Converting data formats
- Renaming columns for consistency
- Ensuring proper data types

---

##  Data Cleaning Process

### 1. Load the Dataset

The dataset is in a **tab-separated format**, so it must be read using appropriate delimiters to correctly load all columns. Excel version was also used to cross-verify formatting.

---

### 2. Handle Missing Values

After checking for null or missing values, it was observed that only the **`Income`** column had missing entries. These missing values were handled by imputing the median income value, ensuring no data loss and maintaining statistical balance.

---

### 3. Remove Duplicate Records

To avoid bias or redundancy in analysis, the dataset was checked for duplicate rows. Any duplicates found were removed to retain only unique records.

---

### 4. Standardize Text Values

Textual categorical fields such as `Marital_Status` and `Education` were reviewed for inconsistencies or unexpected values. For example:
- Marital status values like “YOLO,” “Alone,” or “Absurd” were identified as outliers or unusual entries.
- Education levels were mostly consistent but standardized for consistency across rows.

---

### 5. Convert Date Formats

The column `Dt_Customer` (date of becoming a customer) was converted to a standard **datetime** format (DD-MM-YYYY). This ensures uniformity and proper functioning of time-based operations in later stages.

---

### 6. Rename Column Headers

To improve readability and ensure compatibility with code (e.g., no spaces), all column names were:
- Converted to lowercase
- Replaced spaces with underscores
- Stripped of any leading/trailing whitespaces

This makes the dataset cleaner and easier to handle in programming.

---

### 7. Check and Fix Data Types

All columns were examined to ensure they had the correct data types:
- Numerical values were stored as integers or floats
- Dates were stored in datetime format
- Categorical fields remained as objects

No incorrect types were found after processing.

---

##  Final Dataset Overview

The dataset now contains:
- Cleaned and consistent columns
- No missing or duplicate data
- Properly formatted dates
- Uniform textual categories

This cleaned version is now ready for further analysis such as segmentation, clustering, or predictive modeling.

---

##  About the Dataset

This dataset includes the following types of information:
- Demographics: Age, education, marital status, income, etc.
- Household: Number of kids and teenagers at home
- Purchase behavior: Spending on wine, meat, fish, etc.
- Campaign interaction: Whether a customer accepted a particular campaign
- Web and store interaction: Purchases made via web, catalog, and store

---

##  Tools Used

- **Python (pandas)**
- **Excel**
- **Jupyter Notebook**

---

