# TP03 – Interactive Data Analysis and Visualization with Power BI

University of Eloued – Faculty of Exact Sciences – Department of Computer Science
Master 2 AI & Data Science – Module: Big Data Analytics – 2026/2027

## Dataset
Kaggle: [eCommerce behavior data from multi-category store](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store)
File used: `2019-Nov.csv` (multi-gigabyte, tens of millions of events).
The raw CSV is **not** included because of its size. Only the first **3,000,000 rows** (about 1.5 days, 1-2 November 2019) were loaded into Power BI.

## Contents
| File | Description |
|------|-------------|
| `TP03.pbix` | Power BI report (cleaned data, DAX measures, dashboard) |
| `TP03_report.html` | Report: cleaning steps, before/after screenshots, findings (open in a browser) |
| `images/before1.png`, `images/before2.png` | Imported table before cleaning |
| `images/after1.png`, `images/after2.png` | Table after Power Query cleaning |
| `images/dashboard.png` | Final dashboard screenshot |

## Summary
- Cleaning (Power Query): kept 3M rows, removed `user_session` and `category_id`, converted `event_time` to Date/Time, added `Date`, set data types, replaced empty brand/category by "unknown", split `category_code` into `main_category` and `sub_category`, filtered price > 0, removed duplicates.
- DAX measures: Total Events, Purchases, Revenue, Unique Users, Conversion Rate.
- Dashboard: 3 KPI cards, top 10 brands (bar), events by event type (column), revenue by main category (bar), purchases per hour (line), slicers on event type, main category and brand.

See `TP03_report.html` for the full report and findings.
