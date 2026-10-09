# Build OpenAPI-to-Postman CLI converter

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/7sY9AUcTscrX38TaATawo2c) · delivered as a Markdown file you can import or edit.

OpenAPI-to-Postman CLI Converter - delivered as a Markdown file you can import or edit.

*Product line: Write and license a small software utility*

---

## Preview

# OpenAPI-to-Postman CLI Converter

A tiny, zero‑dependency CLI tool that converts an OpenAPI 3.0/3.1 specification (JSON or YAML) into a Postman Collection v2.1 file. Install with `pip`, run `openapi2postman <spec> [-o <output>]`, and get a ready‑to‑import Postman collection.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Command Reference](#command-reference)
- [Examples](#examples)
- [Development](#development)
- [Testing](#testing)
- [License](#license)

## Features
- ✅ Supports OpenAPI 3.0 and 3.1 (JSON/YAML)
- ✅ Generates Postman Collection v2.1 with folders per tag
- ✅ Handles path, query, header, and cookie parameters
- ✅ Converts `requestBody` (JSON schema) to raw JSON body (example if provided)
- ✅ Maps responses to Postman response objects (status code only)
- ✅ Preserves servers, security schemes (API key only) as environment variables
- ✅ No external dependencies beyond PyYAML (bundled)
- ✅ MIT licensed

## Installation
```bash
# From PyPI (recommended)
pip install openapi2postman==1.0.0

# Or install from source
git clone https://github.com/yourname/openapi2postman.git
cd openapi2postman
pip install -e .
```

## Usage
```bash
openapi2postman SPEC_FILE [-o OUTPUT_FILE] [--pretty]

Arguments:
  SPEC_FILE      Path to OpenAPI spec (JSON or YAML)
  OUTPUT_FILE    Output Postman collection file (default: <spec_basename>.postman_collection.json)
  --pretty       Pretty‑print JSON output (indent 2)
```

### Example
```bash
openapi2postman petstore.yaml -o petstore.postman_collection.json --pretty
```

## Command Reference
| Flag               | Description                                                            |
|--------------------|------------------------------------------------------------------------|
| `-o, --output`     | Path for generated Postman collection. If omitted, uses `<spec>.postman_collection.json` |
| `--pretty`         | Indent output JSON with 2 spaces for readability                      |
| `-h, --help`       | Show help message                                                      |
| `-v, --version`    | Print version and exit                                                 |

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/7sY9AUcTscrX38TaATawo2c)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
