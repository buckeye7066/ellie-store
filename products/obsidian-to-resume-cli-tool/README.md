# Obsidian-to-Resume CLI Tool

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/9B6fZi7z8crXaBlgZhawo0y) · delivered as a Markdown file you can import or edit.


*Product line: code_utility*

---

## Preview

# Obsidian-to-Resume CLI Tool

A tiny, zero‑dependency‑heavy command‑line utility that turns a single Obsidian vault note (written in Markdown with YAML front‑matter) into a polished PDF resume.  
Designed for developers who keep rewriting the same throwaway script and want a reliable, tested tool they can drop into any project.

---  

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Project Structure](#project-structure)
- [Source Code](#source-code)
- [Testing](#testing)
- [License](#license)
- [Changelog](#changelog)

---  

## Overview

The tool expects a single Markdown file that contains:

* YAML front‑matter with structured resume data (name, contact, summary, experience, education, skills).
* The Markdown body is **ignored** for the resume layout – you can keep free‑form notes there if you wish.

It renders the data through a Jinja2 HTML template, then converts that HTML to PDF using **WeasyPrint** (which itself depends on Cairo/Pango/GDK‑Pixbuf but is bundled via pip wheels on major platforms).  

The CLI is built with **Click**, making installation and invocation straightforward.

---  

## Features

| Feature | Description |
|---------|-------------|
| **Simple CLI** | `obsidian-resume resume.md output.pdf` |
| **YAML front‑matter parsing** | Uses `python-frontmatter` to extract resume fields. |
| **Customizable template** | Ship with a clean, A4‑friendly Jinja2 template; users can supply their own via `--template`. |
| **PDF output** | High‑quality vector PDF via WeasyPrint (no headless browser needed). |
| **Zero configuration** | Works out‑of‑the‑box with the bundled template. |
| **Tested** | Unit tests cover front‑matter parsing, template rendering, and PDF generation. |
| **MIT Licensed** | Free to use, modify, and redistribute. |

---  

## Installation

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/9B6fZi7z8crXaBlgZhawo0y)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
