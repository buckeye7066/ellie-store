# Create and sell a short course on 'Automating Excel with Python Pandas'

**Price: $39.00** · [Buy the full pack](https://buy.stripe.com/eVq14oaLk9fLdNx38rawo1a) · delivered as a Markdown file you can import or edit.

Automating Excel with Python Pandas: A 3‑Lesson Drip Course - delivered as a Markdown file you can import or edit.

*Product line: Sell a finite, drip-delivered course*

---

## Preview

# Automating Excel with Python Pandas: A 3‑Lesson Drip Course  

**Target outcome:** By the end of this course you will be able to read any Excel workbook, clean and reshape its data with pandas, and generate a fully‑formatted automated report (new Excel file with multiple sheets, charts, and conditional formatting) using only Python.  

---  

## Lesson 1 – Reading Excel Files & First Look at the Data  

### Video transcript (≈12 min)  

| Timestamp | Content |
|-----------|---------|
| 0:00‑0:45 | **Welcome & learning goals** – “In this lesson you’ll learn how to load an Excel workbook into a pandas DataFrame, inspect its structure, and spot common data‑quality issues.” |
| 0:45‑2:30 | **Sample data walk‑through** – Show the provided `sales_data.xlsx` (see notebook) and explain each column: `Date` (datetime), `Region` (text), `Product` (text), `Units` (int), `Revenue` (float). |
| 2:30‑5:00 | **Reading with pandas** – Demonstrate `pd.read_excel()` with arguments `sheet_name`, `usecols`, `dtype`, `parse_dates`. Show how to load a specific sheet or all sheets into a dict of DataFrames. |
| 5:00‑7:30 | **Quick sanity checks** – Use `.info()`, `.head()`, `.describe()`, `.isnull().sum()`. Explain what each tells you about the data. |
| 7:30‑9:30 | **Basic cleaning** – Convert date column, strip whitespace from text columns, replace missing numeric values with 0 or forward‑fill as appropriate. |
| 9:30‑10:30 | **Exporting a cleaned preview** – Save the cleaned DataFrame to a new Excel file (`cleaned_preview.xlsx`) using `ExcelWriter`. |
| 10:30‑12:00 | **Recap & preview of Lesson 2** – Summarize the workflow and tease the transformation steps coming next. |

### Jupyter Notebook – `Lesson_01_Reading_Data.ipynb`  

```markdown
# Lesson 1: Reading Excel Files & First Look at the Data
```

#### Cell 1 – Imports & settings  
```python
import pandas as pd
import numpy as np
import os

# Ensure reproducible display
pd.set_option('display.max_columns', None)
pd.set_option('display.width', 120)
```

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $39.00](https://buy.stripe.com/eVq14oaLk9fLdNx38rawo1a)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
