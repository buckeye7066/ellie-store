# Curate and sell public API rate limits dataset for top 20 SaaS providers

**Price: $29.00** · [Buy the full pack](https://buy.stripe.com/3cI6oI4mW8bHcJt8sLawo0v) · delivered as a Markdown file you can import or edit.


*Product line: dataset*

---

## Preview

# API Rate Limits Dataset for Top 20 SaaS Providers (v1.0)

## Overview
This dataset compiles publicly documented API rate limits for the top 20 SaaS providers as of **2024-09-28**. Each row includes the provider, service, endpoint, HTTP method, rate limit, limit unit, associated cost tier (if applicable), last‑updated date, and a direct source URL for verification. The data is provided in both CSV and JSON formats, accompanied by a data dictionary, versioning information, and a Creative Commons Attribution 4.0 International license.

## Data Dictionary

| Column Name      | Description                                                                                              | Example                                   |
|------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------|
| provider         | Name of the SaaS company offering the API                                                                | `GitHub`                                  |
| service          | Specific product or API grouping within the provider (if applicable)                                     | `REST API`                                |
| endpoint         | API path (excluding base URL) that the rate limit applies to                                            | `/repos/{owner}/{repo}`                   |
| http_method      | HTTP verb the limit is defined for (GET, POST, PUT, DELETE, PATCH, or `*` for all)                     | `GET`                                     |
| rate_limit       | Maximum number of requests allowed within the limit window                                              | `5000`                                    |
| limit_unit       | Time window for the limit (second, minute, hour, day)                                                   | `hour`                                    |
| cost_tier        | Pricing tier or plan that the limit applies to (e.g., Free, Pro, Enterprise) or `N/A` if universal    | `Free`                                    |
| last_updated     | Date (YYYY‑MM‑DD) when the limit was last verified from the source

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $29.00](https://buy.stripe.com/3cI6oI4mW8bHcJt8sLawo0v)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
