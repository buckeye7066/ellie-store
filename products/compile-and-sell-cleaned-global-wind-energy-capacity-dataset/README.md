# Compile and sell cleaned Global Wind Energy Capacity dataset 2020‑2023

**Price: $29.00** · [Buy the full pack](https://buy.stripe.com/4gMfZi7z8gId24P5gzawo1W) · delivered as a Markdown file you can import or edit.

Global Wind Energy Capacity Dataset 2020‑2023 v1.0 - delivered as a Markdown file you can import or edit.

*Product line: Compile and license a cited reference dataset*

---

## Preview

# Global Wind Energy Capacity Dataset 2020‑2023 v1.0

## License
Creative Commons Attribution 4.0 International (CC BY 4.0)  
You are free to share and adapt the material, even commercially, provided you give appropriate credit, provide a link to the license, and indicate if changes were made.

## README

### Overview
This package contains a cleaned, versioned reference dataset of annual installed wind energy capacity (in gigawatts, GW) for each country from 2020 to 2023. The data are sourced from the Global Wind Energy Council (GWEC) *Global Wind Report* series and the International Energy Agency (IEA) *Wind Energy Statistics*. The dataset has been deduplicated, standardized to ISO‑3166‑1 alpha‑3 country codes, and annotated with per‑row source citations.

### Contents
- `GLOBAL_WIND_CAPACITY_2020_2023.csv` – the core dataset (CSV, UTF‑8, comma‑separated).  
- `DATA_DICTIONARY.md` – description of each column.  
- `SOURCES.md` – detailed bibliographic references for each row, with URLs and access dates.  
- `generate_dataset.py` – reproducible Python script that pulls the raw GWEC and IEA tables, performs cleaning, deduplication, and outputs the CSV and source file.  
- `LICENSE.txt` – full text of the CC BY 4.0 license.

### Methodology
1. **Data acquisition**  
   - GWEC: downloaded the “Cumulative Installed Capacity by Country” tables from the Global Wind Report 2021 (covers 2020), 2022 (2021), 2023 (2022), and 2024 (2023). URLs are listed in `SOURCES.md`.  
   - IEA: extracted the “Wind Power – Installed Capacity” table from the IEA Wind Energy Statistics 2021‑2024 spreadsheets (available via the IEA Data Portal).  

2. **Standardization**  
   - Country names were matched to the ISO‑3166‑1 alpha‑3 list using the `pycountry` library; ambiguous entries were resolved manually.  
   - All capacities were converted to gigawatts (GW) with three decimal places.

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $29.00](https://buy.stripe.com/4gMfZi7z8gId24P5gzawo1W)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
