# Compile and sell US public EV charging utilization CSV 2024

**Price: $29.00** · [Buy the full pack](https://buy.stripe.com/fZueVe4mW63zdNxfVdawo1g) · delivered as a Markdown file you can import or edit.

US Public EV Charging Utilization CSV 2024 - v1.0 - delivered as a Markdown file you can import or edit.

*Product line: Compile and license a cited reference dataset*

---

## Preview

# US Public EV Charging Utilization CSV 2024 - v1.0

## Data Dictionary

| Column Name | Description | Type | Unit | Source |
|-------------|-------------|------|------|--------|
| station_id | Unique identifier from Open Charge Map | string | - | OCM API |
| station_name | Name of the charging station | string | - | OCM API |
| latitude | Decimal degrees latitude | float | degrees | OCM API |
| longitude | Decimal degrees longitude | float | degrees | OCM API |
| address | Street address | string | - | OCM API |
| city | City | string | - | OCM API |
| state | US state abbreviation | string | - | OCM API |
| zip_code | Postal code | string | - | OCM API |
| date | Date of observation (YYYY-MM-DD) | string | date | OCM API |
| hour | Hour of day (0-23) | integer | hour (local time) | OCM API |
| utilization_percent | Percentage of charging ports in use during that hour | float | % | OCM API |
| source_url | Direct API endpoint used for this row (API key omitted) | string | - | OCM API |

## License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0). To view a copy of this license, visit <http://creativecommons.org/licenses/by/4.0/>.

## Source Code

```python
#!/usr/bin/env python3
"""
Generate US public EV charging utilization CSV for 2024 from Open Charge Map API.
Requires an OCM API key (set as environment variable OCM_API_KEY).
Outputs: ev_charging_utilization_2024_v1.0.csv
"""

import os
import requests
import pandas as pd
from datetime import datetime, timedelta

API_KEY = os.getenv("OCM_API_KEY")
if not API_KEY:
    raise EnvironmentError("Please set the OCM_API_KEY environment variable.")

BASE_URL = "https://api.openchargemap.io/v3/poi/"
PARAMS = {
    "output": "json",
    "countrycode": "US",
    "maxresults": 5000,  # adjust as needed; paginate if more
    "compact": "true",
    "verbose": False,
    "key": API_KEY
}

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $29.00](https://buy.stripe.com/fZueVe4mW63zdNxfVdawo1g)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
