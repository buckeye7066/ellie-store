# Build and sell Notion OKR tracking template

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/28EeVebPo8bHfVF24nawo0x) · delivered as a Markdown file you can import or edit.


*Product line: code_utility*

---

## Preview

# Notion OKR Tracking Template  

## Overview  
This template provides a complete OKR (Objectives and Key Results) system for weekly tracking inside Notion. It includes two linked databases: **Objectives** and **Key Results**, plus a **Weekly Progress** view that rolls up progress from Key Results into each Objective. The template comes with predefined properties, formulas, filters, sorts, and sample data so you can start using it immediately after import.

---

## Database Schema  

### 1. Objectives Database  
| Property | Type | Description | Example |
|----------|------|-------------|---------|
| Name | Title | Objective statement | "Improve website performance" |
| Description | Text | Detailed description | "Reduce load time <2s on mobile" |
| Owner | Person | Team member responsible | @Alice |
| Due Date | Date | Target completion date | 2025-12-31 |
| Status | Select | Progress status | `Not Started`, `In Progress`, `Done` |
| Priority | Select | Importance level | `High`, `Medium`, `Low` |
| Progress | Formula | Roll‑up of Key Results completion (%) | `round(prop("Key Results Progress") * 100) / 100` |
| Key Results Progress | Rollup | Average of linked Key Results' % Complete | (see KR database) |
| Weekly Check‑in | Relation | Link to Weekly Progress entries (auto‑filled) | — |
| Tags | Multi‑label | Custom labels for grouping | `Performance`, `UX` |
| Created Time | Created Time | Auto‑timestamp | — |
| Last Edited Time | Last Edited Time | Auto‑timestamp | — |

**Formula for Progress** (copy exactly):  
```
round(prop("Key Results Progress") * 100) / 100
```

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/28EeVebPo8bHfVF24nawo0x)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
