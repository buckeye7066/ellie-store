# Create and sell a JSON schema CLI validator

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/00wbJ2bPo2RnaBl9wPawo2b) · delivered as a Markdown file you can import or edit.

jsonschema-cli - delivered as a Markdown file you can import or edit.

*Product line: Write and license a small software utility*

---

## Preview

# jsonschema-cli

A tiny command‑line utility for validating JSON files against a JSON Schema. Install with `pip install jsonschema-cli` and run `jsonschema-cli validate <schema> <data>`.

## Installation

```bash
pip install jsonschema-cli
```

## Usage

Validate a JSON document:

```bash
jsonschema-cli validate schema.json data.json
```

If the data is valid the command exits with status 0 and prints nothing.  
If validation fails, an error message is printed to stderr and the exit status is 1.

Show help:

```bash
jsonschema-cli --help
```

## Development

Clone the repo, create a virtualenv, install dev dependencies and run tests:

```bash
git clone https://github.com/yourname/jsonschema-cli.git
cd jsonschema-cli
python -m venv .venv
source .venv/bin/activate
pip install -e ".[test]"
pytest
```

## License

MIT License (see `LICENSE` file).

---

### File tree

```
jsonschema-cli/
├── jsonschema_cli/
│   ├── __init__.py
│   └── __main__.py
├── tests/
│   └── test_cli.py
├── LICENSE
├── README.md
├── pyproject.toml
└── setup.cfg
```

---

### jsonschema_cli/__init__.py

```python
"""Top-level package for jsonschema-cli."""

__author__ = "Your Name"
__email__ = "you@example.com"
__version__ = "0.1.0"
```

---

### jsonschema_cli/__main__.py

```python
#!/usr/bin/env python
"""Console script for jsonschema-cli."""
import argparse
import json
import sys

import jsonschema
from jsonschema import ValidationError


def _build_parser() -> argparse.ArgumentParser:
    parser = argparse.ArgumentParser(
        description="Validate a JSON document against a JSON Schema."
    )
    parser.add_argument(
        "schema",
        help="Path to the JSON Schema file.",
    )
    parser.add_argument(
        "data",
        help="Path to the JSON data file to validate.",
    )
    return parser


def main(argv=None) -> int:
    parser = _build_parser()
    args = parser.parse_args(argv)

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/00wbJ2bPo2RnaBl9wPawo2b)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
