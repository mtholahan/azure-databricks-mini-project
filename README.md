# Azure Mini Project 01: Databricks Lab

**Springboard Data Engineering Boot Camp**  
Author: Mark Holahan  
Project Type: Mini Project  
Platform: Azure Databricks  
Tools: PySpark, Databricks, Spark DataFrames

---

## 📘 Overview

This project demonstrates the use of **Azure Databricks** and **native PySpark syntax** to ingest, clean, and analyze structured banking datasets. The exercise was completed as part of the Springboard Data Engineering Boot Camp and reinforces foundational big data processing techniques using Apache Spark.

---

## 🛠️ Technologies Used

| Tool/Platform    | Purpose                                |
| ---------------- | -------------------------------------- |
| Azure Databricks | Interactive notebooks + compute engine |
| PySpark          | Data transformation and querying       |
| Apache Spark     | Distributed data processing            |
| VS Code          | Local editing and QA                   |
| Git + GitHub     | Version control and project tracking   |

---

## 📂 Project Structure

```bash
azure-mini-project-01/
├── banking_lab.ipynb        # Main notebook with all PySpark queries
├── data/
│   ├── loan.csv
│   ├── credit card.csv
│   └── txn.csv
├── README.md
└── .gitignore
```



## 📊 Datasets Used

Three CSV files were used to simulate a multi-domain banking environment:

- `loan.csv`: Customer loan details (e.g., income, loan category, cheque return, etc.)
- `credit card.csv`: Credit eligibility, salary, and account metadata
- `txn.csv`: Transaction-level data including deposits and withdrawals



## ✅ Goals

Each dataset was used to answer specific business questions using **PySpark**:

- Schema introspection (`.printSchema()`)
- Filtering based on conditions (`.filter()`)
- Aggregations (`.agg()`, `.groupBy()`)
- Distinct record counts
- Customer segmentation (by income, location, activity, etc.)

All logic was implemented using PySpark DataFrame syntax, not SQL.

## 🔍 Sample Queries

```python
# Number of customers with income > 60,000
loan_df.filter(col("Income") > 60000).count()

# Maximum withdrawal per account
txn_df.groupBy("ACCOUNT NO").agg(max("WITHDRAWAL AMT")).show()
```

## 📈 Summary

All analytical prompts were completed using native PySpark syntax.
The notebook reflects clean, well-structured, and readable logic with verified outputs.
Compute was shut down after use to minimize costs.



## 📌 Notes

- All queries were validated by manual re-run.
- GitHub Copilot suggestions were reviewed and confirmed for accuracy.
- The notebook was QA'd offline using VS Code's native Jupyter support.

## 📎 Related Repositories

This repo is part of a larger meta-repo:

🔗 [capstone-meta-repo](https://github.com/mtholahan/Springboard-Projects) *(replace with actual URL)*
