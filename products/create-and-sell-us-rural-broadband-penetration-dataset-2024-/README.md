# Create and sell US rural broadband penetration dataset 2024-2025

**Price: $29.00** · [Buy the full pack](https://buy.stripe.com/bJe00kg5EeA510L5gzawo1r) · delivered as a Markdown file you can import or edit.

US Rural Broadband Penetration Dataset 2024-2025 (County-Level) - delivered as a Markdown file you can import or edit.

*Product line: Compile and license a cited reference dataset*

---

## Preview

# US Rural Broadband Penetration Dataset 2024-2025 (County-Level)

## Version
1.0.0 (2025-09-16)

## License
Creative Commons Attribution 4.0 International (CC BY 4.0)

## Source Citation
Data derived from FCC Form 477 broadband deployment statistics, fixed terrestrial broadband connections >=25/3 Mbps, accessed via FCC Broadband Deployment Map API and public CSV files for December 2023 (released 2024) and June 2024 (released 2025). Specific files:
- FCC Form 477, V1 Broadband Deployment Data, December 2023: https://www.fcc.gov/general/form-477-broadband-deployment-data
- FCC Form 477, V1 Broadband Deployment Data, June 2024: https://www.fcc.gov/general/form-477-broadband-deployment-data
Accessed on 2025-09-15.

## Data Dictionary
| Column Name | Description | Type | Example |
|-------------|-------------|------|---------|
| state_fips | Two‑digit FIPS code for the state | string | "01" |
| county_fips | Three‑digit FIPS code for the county | string | "001" |
| fips | Five‑digit FIPS code (state+county) | string | "01001" |
| county_name | Name of the county | string | "Autauga County" |
| state_name | Name of the state | string | "Alabama" |
| year | Year of the measurement (2024 or 2025) | integer | 2024 |
| broadband_penetration_pct | Percentage of households with fixed terrestrial broadband ≥25/3 Mbps | numeric (0‑100) | 78.5 |
| source_url | Direct link to the FCC Form 477 file used for this row | string | "https://www.fcc.gov/e.../dec2023.csv" |
| retrieval_date | Date the source file was downloaded | date (YYYY‑MM‑DD) | 2025-09-10 |

## Reproduction Steps
1. Install Python ≥ 3.9 and required packages:
   ```bash
   pip install pandas requests tqdm
   ```
2. Save the script below as `build_broadband_dataset.py`.
3. Run the script:
   ```bash
   python build_broadband_dataset.py
   ```
4. The script will output `us_rural_broadband_2024_2025.csv` in the current directory.
5. (Optional) Validate the output with the provided data dictionary.

### Build Script (`build_broadband_dataset.py`)
```python
import pandas as pd
import requests
import io
import os
from tqdm import tqdm

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $29.00](https://buy.stripe.com/bJe00kg5EeA510L5gzawo1r)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
