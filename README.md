# SWYNEX-Data-Cleaning-Preparation
# Task 1 — Data Cleaning & Preparation

## Overview

This project was completed as **Task 1 of my internship project**.

The objective was to inspect a raw dataset, identify data-quality issues, and prepare the dataset for further analysis using **Microsoft Excel Online**.

The cleaning process focused on:

* Missing and incomplete values
* Duplicate records
* Incorrect or inconsistent data types
* Inconsistent categorical values
* Date formatting


## Tool Used

**Microsoft Excel Online**

---

## Data Cleaning Process

### 1. Missing / Incomplete Values

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

## 2. Duplicate Records

I checked the dataset for duplicate records.

**Result:**

* Duplicate records found: **0**

No duplicate records were identified during the duplicate check.


## 3. Data Type Validation

I reviewed the data types and number formats of the dataset columns.

Examples:

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

## 4. Date Standardization

The date column contained inconsistent date representations.

I standardized the dates into the following format:

**DD-MM-YYYY**

Example:

`18-04-2008`

This makes the date values easier to read and keeps the dataset consistent for future analysis.

## 5. Inconsistent Value Check

I checked categorical columns for:

* Different spellings
* Different capitalization
* Duplicate names written in different ways
* Unnecessary variations
* Unexpected categorical values

### Columns checked

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

## Key Findings

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

## Project Objective

The purpose of this task was not simply to modify values, but to understand the quality of a raw dataset before using it for analysis.

The workflow followed was:

**Raw Dataset → Data Quality Check → Missing Value Identification → Duplicate Check → Data Type Validation → Date Standardization → Inconsistency Check → Prepared Dataset**

## Skills Demonstrated

* Microsoft Excel Online
* Data Cleaning
* Data Preparation
* Missing Value Identification
* Duplicate Detection
* Data Type Validation
* Date Standardization
* Categorical Data Validation
* Data Quality Documentation

## Project Outcome

The dataset was systematically reviewed and prepared for subsequent data analysis.

This project provided practical experience in identifying common data-quality problems that can affect analysis and reporting.

IPL-Data-Cleaning/
│
├── README.md
│
├── IPL_MATCHES_RAW_DATA:[IPL_Matches_Data_2008_2026 1(Sheet1).csv]
│
└── IPL_Matches_Data_2008_2026: [IPL_Matches_Data_2008_2026 1.pdf]

Internship Task
**Task:** Task 1 — Data Cleaning & Preparation
Tool: Microsoft Excel Online
Status: Completed
**Tool:** Microsoft Excel Online
**Status:** Completed
