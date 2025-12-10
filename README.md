# Fuzzy Matching Data Imputation (Jupyter Notebook)

This repository contains a single Jupyter Notebook that performs **fuzzy matching–based data imputation** on Excel datasets.  
The notebook identifies missing values in selected columns and fills them by finding the closest match based on a reference text column (for example, agency names or customer names).

---

## 📌 What the Notebook Does

- Loads an input Excel file  
- Identifies missing values in specific columns  
- Uses **FuzzyWuzzy** to find best string matches  
- Replaces missing values with match results  
- Assigns `"No Match"` when match score is too low  
- Exports a cleaned Excel file  
- Keeps all configuration safe and generic (no personal paths or sensitive data included)

---

## 📁 Notebook Purpose

This notebook is designed to help:
- Clean master data files  
- Automatically fix incomplete records  
- Standardize text-based groups  
- Improve dataset consistency before analysis  

It works well for:
- Customer lists  
- Agency or vendor lists  
- Product groups  
- Organizational mapping  
- Any Excel file with missing labels  

---

## 🔧 Requirements

Install the required packages:

```bash
pip install pandas fuzzywuzzy python-Levenshtein
