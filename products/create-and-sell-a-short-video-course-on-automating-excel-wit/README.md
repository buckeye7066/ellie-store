# Create and sell a short video course on 'Automating Excel with Python and OpenPyXL'

**Price: $39.00** · [Buy the full pack](https://buy.stripe.com/eVqbJ23iS77DdNx6kDawo1T) · delivered as a Markdown file you can import or edit.

Automating Excel with Python and OpenPyXL - delivered as a Markdown file you can import or edit.

*Product line: Sell a finite, drip-delivered course*

---

## Preview

# Automating Excel with Python and OpenPyXL  

## Lesson 1: Course Overview and Prerequisites (5 min)  

**Learning Objectives**  
- Explain what OpenPyXL does and why it is useful for automating Excel tasks.  
- List the software versions required to follow along.  
- Set up a working Python environment.  

**Key Points**  
- OpenPyXL is a pure‑Python library for reading and writing `.xlsx` files (Excel 2010+).  
- It lets you manipulate worksheets, cells, styles, charts, and more without launching Excel.  
- No prior experience with OpenPyXL is required, but basic Python syntax (variables, loops, functions) is assumed.  

**Setup Checklist**  

| Item | Minimum Version | How to Verify |
|------|----------------|---------------|
| Python | 3.8+ | `python --version` |
| pip | 20.0+ | `pip --version` |
| OpenPyXL | 3.1.2+ | `pip show openpyxl` |
| Code editor (VS Code, PyCharm, etc.) | any | open editor |
| Sample data file (`sales_sample.xlsx`) | – | download from link below |

**Download Sample File**  
[Sales Sample Excel File](https://example.com/sales_sample.xlsx) (right‑click → Save As). The file contains three sheets: `Jan`, `Feb`, `Mar`, each with columns `Date`, `Product`, `Units Sold`, `Unit Price`, `Total`.

**Quick Test**  
Create a file `test_openpyxl.py` with the following code and run it:

```python
import openpyxl
wb = openpyxl.load_workbook('sales_sample.xlsx')
print(wb.sheetnames)   # Should output ['Jan', 'Feb', 'Mar']
wb.close()
```

If you see the sheet names printed, your environment is ready.  

---  

## Lesson 2: Reading Excel Files (7 min)  

**Learning Objectives**  
- Load a workbook and select a worksheet.  
- Retrieve cell values using coordinate and iterative methods.  
- Convert worksheet data into Python structures (lists, dictionaries).  

**Core Concepts**  

- `openpyxl.load_workbook(filename, read_only=True)` – opens file in read‑only mode for large files.  
- `ws['A1']` or `ws.cell(row=1, column=1)` – access a single cell.  
- `ws.iter_rows(min_row, max_row, min_col, max_col, values_only=True)` – efficient row‑wise iteration.  

**Step‑by‑Step: Reading the Jan Sheet**  

1. Import and open workbook (read‑only for speed).

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $39.00](https://buy.stripe.com/eVqbJ23iS77DdNx6kDawo1T)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
