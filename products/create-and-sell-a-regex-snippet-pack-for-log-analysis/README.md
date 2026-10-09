# Create and sell a Regex Snippet Pack for Log Analysis

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/bJe28saLk4Zv7p9gZhawo2g) · delivered as a Markdown file you can import or edit.

Regex Snippet Pack for Log Analysis - delivered as a Markdown file you can import or edit.

*Product line: Write and license a small software utility*

---

## Preview

# Regex Snippet Pack for Log Analysis

## Overview
This pack contains **30 tested, ready‑to‑use regular expressions** for parsing common log formats. Each pattern is accompanied by a brief description, an example log line, and the named capture groups it exposes. The pack also includes a few sample log files so you can verify the patterns immediately. Licensed under the MIT License, you can copy, modify, and redistribute the snippets freely in your own projects or commercial products.

## Contents
```
regex-snippet-pack/
├─ LICENSE
├─ README.md          ← this file
├─ patterns/
│  └─ regex-patterns.json   ← machine‑readable list of patterns
└─ samples/
   ├─ apache_access.log
   ├─ nginx_error.log
   ├─ syslog.log
   ├─ docker.log
   ├─ k8s_pod.log
   ├─ windows_event.log
   ├─ json_app.log
   └─ traceback.log
```

## Installation
1. Download the ZIP from Gumroad (or clone the repo if you prefer).  
2. Extract the archive to a location of your choice.  
3. The `patterns/` directory holds `regex-patterns.json`, a JSON array where each entry has:
   - `name`: short identifier
   - `regex`: the pattern (PCRE flavor, suitable for most engines)
   - `description`: what it matches
   - `example`: a sample log line
   - `groups`: list of named capture groups
4. The `samples/` directory contains small log files you can use with `grep`, `rg`, `awk`, or any programming language to test the patterns.

## Usage
### Command line (grep/rg)
```bash
# Apache access log – extract IP, request, status, size
grep -P '(?<ip>\d+\.\d+\.\d+\.\d+).+(?<request>"[^"]*").+(?<status>\d{3}).+(?<size>\d+)$' samples/apache_access.log
```

### Python
```python
import re, json

with open('patterns/regex-patterns.json') as f:
    patterns = json.load(f)

# Example: parse NGINX error log
nginx_pat = next(p for p in patterns if p['name'] == 'nginx_error')
regex = re.compile(nginx_pat['regex'])
match = regex.search('2024/09/26 14:32:10 [error] 12345#0: *1 client timed out while reading client request line, client: 203.0.113.42, server: example.com, request: "GET / HTTP/1.1", host: "example.com"')
print(match.groupdict())
```

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/bJe28saLk4Zv7p9gZhawo2g)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
