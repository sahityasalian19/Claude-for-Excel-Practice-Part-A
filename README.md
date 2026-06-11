# Claude-for-Excel-Practice: Part A

# 🧹 Data Cleaning Practice with Claude AI

A hands-on data cleaning project where I generated a messy dataset using Claude followed by its step-by-step instructions to clean and prepare a Cleaned dataset using **Power Query** from Excel.

---

## 📌 Project Overview

This project documents my practice of essential data cleaning techniques on a raw Excel dataset. The goal was to transform messy, inconsistent data into a clean, analysis-ready format — guided by Claude AI throughout the process.

## 💡Prompts Used

- Generate a messy data with 1000 rows for practice purpose of a tourism company. Create a messy data in such a way that it should look like a real world dataset.
- Give a clear Data Cleaning steps to follow to clean this messy data in power query

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Data inspection and reviewing results |
| Power Query | All data transformations — fixing data types, standardizing formats, renaming columns, outlier detection, creating flag columns etc |

---

## 🔧 Techniques Practiced

### 1. 🔢 Validating/Fixing Data Types
- In most of the case Power Query itself will apply Data type Transformations, also validated from  my end to check the correctness.
- After validating, Applied proper types in Power Query using **Clicking the Data type format near the Column name**

### 2. 📐 Standardizing Formats
- Standardized inconsistent text values by using **Transform→Replace Values**  (e.g., `"male"`, `"Male"`, `"f"` → `"F"`). If multiple replacement then created a custom column with If condition and later deleted the original one.
- Trimmed extra whitespace from text fields using **Transform→Format→Trim** 
- Capitalized texts as for specific columns using **Transform→Format→Capitalize Each Word**

### 3. 📊 Outlier Detection
- Identified outliers in Age (1, 0, 150, 999), Travel Date (Travel date should not be earlier than Booking date) and Customer Rating (0, 6, 9, 10, -1; As per the company rules customer rating should be between 1-5) columns, etc.
- Flagged suspicious values for review rather than blindly removing them

### 4. 🚩 Created Flag Columns
- Added new indicator columns to mark rows with missing values, outliers, or anomalies
- This makes it easy to filter out bad or suspicious rows later when building reports or Pivot Tables

### 5. 🏷️ Renaming Columns
- Renamed cryptic or inconsistent column headers to clear, descriptive names
- Applied a consistent naming convention throughout the dataset

---

## 📁 Project Structure

```
📦 data-cleaning-practice
 ┣ 📂 raw_data
 ┃ ┗ 📄 raw_dataset.xlsx          # Original uncleaned dataset
 ┣ 📂 cleaned_data
 ┃ ┗ 📄 cleaned_dataset.xlsx     # Final cleaned output
```

---

## 💡 Key Learnings

- Data cleaning is rarely a one-step process — it requires inspecting, transforming, and validating iteratively
- Power Query makes repetitive transformations fast and reproducible
- Creating flag columns is a safer approach than deleting uncertain data outright
- Consistent naming and formatting makes downstream analysis significantly easier

---

## 🤖 How Claude AI Helped

Claude provided clear, step-by-step instructions for each cleaning task — from spotting data quality issues to applying the right Power Query transformations. This project was a guided practice session to build real-world data cleaning skills.

---

## 🚀 Next Steps

- [ ] Create reports using pivot table 


---

