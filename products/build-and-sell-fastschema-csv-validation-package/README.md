# Build and sell fastschema CSV validation package

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/eVq5kE7z877DaBl10jawo1z) · delivered as a Markdown file you can import or edit.

fastschema - delivered as a Markdown file you can import or edit.

*Product line: Write and license a small software utility*

---

## Preview

# fastschema

Fast, lightweight CSV schema validation for data engineers.

## Installation

```bash
pip install fastschema
```

## Usage

```python
import csv
from fastschema import validate_csv

schema = {
    "id": {"type": "int", "required": True},
    "name": {"type": "str", "required": True, "max_length": 50},
    "age": {"type": "int", "required": False, "minimum": 0, "maximum": 120},
    "email": {"type": "str", "required": False, "format": "email"},
}

with open("data.csv", newline="") as f:
    reader = csv.DictReader(f)
    for i, row in enumerate(reader, start=1):
        try:
            validate_csv(row, schema)
        except ValueError as e:
            print(f"Row {i} invalid: {e}")
```

## Running Tests

```bash
pytest
```

## License

MIT License. See LICENSE file.

```text
MIT License

Copyright (c) 2025 fastschema author

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

```toml
[build-system]
requires = ["setuptools>=61.0", "wheel"]
build-backend = "setuptools.build_meta"

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/eVq5kE7z877DaBl10jawo1z)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
