# SWYNEX — Data Cleaning & Preparation

## Task 1 — Data Cleaning & Preparation

### Overview

This project was completed as **Task 1 of my SWYNEX internship project**.

The objective was to inspect a raw IPL match dataset, identify data-quality issues, and prepare the dataset for further analysis using **Microsoft Excel Online**.

The cleaning process focused on:

* Missing and incomplete values
* Duplicate records
* Data type validation
* Inconsistent categorical values
* Date formatting


## Tool Used

**Microsoft Excel Online**

## Dataset

The project uses an **IPL match dataset** containing information related to seasons, match numbers, dates, venues, teams, toss decisions, results, players, and umpires.

---
## Project Files


* 📊 **[View / Download IPL Raw Dataset (CSV)](IPL_RAW_DATA.csv)**
* 📄 **[View IPL Dataset Reference (PDF)](IPL_CLEANED_OUTPUT.pdf)**


### File Description

| File                                       | Description                                             |
| ------------------------------------------ | ------------------------------------------------------- |
| `IPL_Matches_Data_2008_2026 1(Sheet1).csv` | Raw IPL match dataset used for the data-cleaning task   |
| `IPL_Matches_Data_2008_2026 1.pdf`         | PDF reference/documentation for the IPL dataset         |
| `README.md`                                | Documentation of the data-cleaning process and findings |

---

# Data Cleaning Process

## 1. Missing / Incomplete Values

I inspected the dataset for values such as `N/A`, `None`, and `Unknown`.

The following findings were identified:

| Column                | Missing / Incomplete Value | Count |
| --------------------- | -------------------------- | ----: |
| `MATCH_NUMBER`        | `N/A`                      |    74 |
| `WINNER`              | `None`                     |    25 |
| `PLAYER_OF_THE_MATCH` | `None`                     |     9 |
| `CITY`                | `Unknown`                  |    53 |
| `TV_UMPIRE`           | `Unknown`                  |     4 |
| `RESERVE_UMPIRE`      | `Unknown`                  |    24 |

`N/A` was treated as an unavailable or unprovided value rather than replacing it with an invented number.

The `None` and `Unknown` values were documented rather than blindly replaced because their meaning depends on the context of the original dataset.

---

## 2. Duplicate Records

I checked the dataset for duplicate records.

**Result:**

* Duplicate records found: **0**

No duplicate records were identified during the duplicate check.

---

## 3. Data Type Validation

I reviewed the data types and number formats of the dataset columns.

| Column          | Data Type / Format | Result       |
| --------------- | ------------------ | ------------ |
| `DATE`          | Date               | Standardized |
| `SEASON`        | Number             | No issue     |
| `MATCH_NUMBER`  | General            | Appropriate  |
| `TEAM1`         | General            | Appropriate  |
| `TEAM2`         | General            | Appropriate  |
| `VENUE`         | General            | Appropriate  |
| `CITY`          | General            | Appropriate  |
| `TOSS_WINNER`   | General            | Appropriate  |
| `TOSS_DECISION` | General            | Appropriate  |
| `RESULT_TYPE`   | General            | Appropriate  |

No unnecessary data-type changes were made where the existing format was appropriate.

---

## 4. Date Standardization

The `DATE` column contained inconsistent date representations.

I standardized the dates into the following format:

**DD-MM-YYYY**

### Example

`18-04-2008`

This provides a consistent date format for future analysis.

---

## 5. Inconsistent Value Check

I checked categorical columns for:

* Different spellings
* Different capitalization
* Duplicate names written in different ways
* Unnecessary variations
* Unexpected categorical values

### Columns Checked

* `TOSS_DECISION`
* `RESULT_TYPE`
* `WINNER`
* `PLAYER_OF_THE_MATCH`
* `TV_UMPIRE`
* `RESERVE_UMPIRE`
* `UMPIRE1`
* `UMPIRE2`

### Findings

No additional spelling or capitalization inconsistencies were identified during the checks.

For example, `TOSS_DECISION` contained:

* `bat`
* `field`

`RESULT_TYPE` contained:

* `complete`
* `no result`
* `tie`

These values were consistently represented in the dataset.

---

# Key Findings

The data-quality assessment identified:

* **74** `N/A` values in `MATCH_NUMBER`
* **25** `None` values in `WINNER`
* **9** `None` values in `PLAYER_OF_THE_MATCH`
* **53** `Unknown` values in `CITY`
* **4** `Unknown` values in `TV_UMPIRE`
* **24** `Unknown` values in `RESERVE_UMPIRE`
* **0 duplicate records**
* Date formatting standardized to **DD-MM-YYYY**
* No additional categorical spelling/capitalization inconsistencies found during the review

---

# Data Cleaning Workflow

```text
Raw IPL Dataset
       ↓
Data Quality Check
       ↓
Missing Value Identification
       ↓
Duplicate Check
       ↓
Data Type Validation
       ↓
Date Standardization
       ↓
Inconsistency Check
       ↓
Prepared Dataset
```

# Skills Demonstrated

* Microsoft Excel Online
* Data Cleaning
* Data Preparation
* Missing Value Identification
* Duplicate Detection
* Data Type Validation
* Date Standardization
* Categorical Data Validation
* Data Quality Documentation

# Project Outcome

The IPL dataset was systematically reviewed for common data-quality issues and prepared for subsequent data analysis.

This project provided practical experience in identifying and documenting data-quality problems that can affect analysis and reporting.

# Internship Information

**Internship:** SWYNEX
**Task:** Task 1 — Data Cleaning & Preparation
**Dataset:** IPL Match Data
**Tool:** Microsoft Excel Online
**Status:** Completed

