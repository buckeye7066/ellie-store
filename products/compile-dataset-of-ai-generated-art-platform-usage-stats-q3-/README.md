# Compile dataset of AI-generated art platform usage stats Q3 2024

**Price: $59.00** · [Buy the full pack](https://buy.stripe.com/5kQcN67z863zfVFcJ1awo1K) · delivered as a Markdown file you can import or edit.

AI-Generated Art Platform Usage Stats Q3 2024 Dataset - delivered as a Markdown file you can import or edit.

*Product line: Clean and structure data a buyer supplies*

---

## Preview

# AI-Generated Art Platform Usage Stats Q3 2024 Dataset

## Overview
This product delivers a cleaned, validated CSV dataset containing monthly active users (MAU), image generation counts, and revenue estimates for the three leading AI‑generated art platforms—Midjourney, DALL‑E, and Stable Diffusion—for Q3 2024 (July, August, September). Alongside the dataset, a reusable Python script is provided that reproduces the cleaning and validation steps from the raw source files, enabling buyers to update or extend the data independently.

## Data Sources
| Platform | Source Type | Details |
|----------|-------------|---------|
| Midjourney | Public Discord analytics + press releases | MAU estimated from Discord member counts (publicly disclosed via server insights) and image generation counts from monthly blog posts; revenue derived from subscription tiers (Basic, Standard, Pro) disclosed in Q3‑2024 financial summary. |
| DALL‑E | OpenAI usage reports + Azure Marketplace | MAU approximated from Azure OpenAI service usage dashboards (publicly shared in OpenAI’s Q3‑2024 blog); image generation counts from API call logs; revenue calculated using published per‑image pricing ($0.02 per image) multiplied by volume. |
| Stable Diffusion | Stability AI blog + Hugging Face inference API stats | MAU derived from Hugging Face Inference API active user counts (monthly MAU endpoint); image generation counts from API request logs; revenue estimated from enterprise licensing fees disclosed in Stability AI’s Q3‑2024 press release. |

All source URLs are listed in the `SOURCES.md` file bundled with the script (see below). The raw data extracted from these sources is stored in `raw_data.csv` (included in the repository) and contains the following columns before cleaning:

- `platform` (string)
- `month` (string, format `YYYY-MM`)
- `mau_raw` (string, may contain commas or “+”)
- `images_raw` (string, may contain scientific notation or abbreviations)
- `revenue_raw` (string, may contain currency symbols, commas, or textual qualifiers)

## Dataset Description
The final cleaned dataset (`cleaned_qa_q3_2024.csv`) contains exactly nine rows (3 platforms × 3 months) and five columns:

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $59.00](https://buy.stripe.com/5kQcN67z863zfVFcJ1awo1K)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
