# Performance Analysis Dashboard

⚠️ **Sensitive data notice:** This dashboard includes performance ratings, manager ratings, and PIP (Performance Improvement Plan) status broken down by department, job profile, and business unit. Even in aggregate, this can reflect on individual managers or small teams. Consider keeping this repo **private**, or replace real figures with synthetic data before publishing.

A Power BI dashboard analyzing employee performance — high/low performer rates, promotion trends, goal achievement, and PIP status — to support performance management and calibration.

https://github.com/Manisha-mishra-visualization/Performance-Analysis-Dashboard/blob/main/overview_dashboard.png

## Overview

Performance analytics dashboard tracking ratings, promotions, and PIP status across departments, job profiles, and business units. Covers 80 high performers, 26 low performers, 38 employees on PIP, an average rating of 3.26, and 486 goals achieved, with filters for department, manager rating, promotion, and PIP status. Built in Power BI with DAX.

## Key Metrics

| Metric | Value |
|---|---|
| High Performer | 80 |
| Low Performer | 26 |
| PIP | 38 |
| Average Rating | 3.26 |
| Goal Achieved | 486 |
| Promotion | 18 |

## Dashboard Sections

- **Performance by Department** — table showing High Performer Rate, Low Performer Rate, PIP Rate, Promotion Rate, Goal Achievement Rate, Average Manager Rating, and Average Rating across Finance, HR, IT, Marketing, Operations, and Sales, with totals.
- **Promotion Rate by Job Profile** — bar chart across roles: Senior Director, Senior Associate, Director, Manager, Specialist, Senior Manager, Analyst, and Senior Analyst.
- **Performance by Business Unit** — clustered bar chart of Goal Achieved, High Performer, Low Performer, and PIP counts across Corporate, Commercial, Operations, and Technology.
- **High Performer Rate vs. Low Performer Rate by Department** — horizontal comparison bars across Operations, Finance, IT, HR, Marketing, and Sales.

## Filters

- **Department** — filter all visuals by department.
- **Manager Rating** — filter all visuals by manager rating.
- **Promotion Status** — filter all visuals by promotion status.
- **PIP Status** — filter all visuals by PIP status.

## Tech Stack

- **Power BI Desktop** — dashboard authoring
- **Power Query (M)** — data transformation
- **DAX** — calculated measures (see [docs/dax_measures.md](docs/dax_measures.md))

## Data

> **No real employee performance data is included in this repository.** Place your own dataset in `data/raw/` before opening the `.pbix` file, or point Power BI to your own data source. See [docs/data_dictionary.md](docs/data_dictionary.md) for expected columns.

## Repository Structure

```
Performance-Analysis-Dashboard/
├── data/
│   ├── raw/            # original/source dataset — sensitive, do not commit real data
│   └── processed/      # cleaned data used by the model
├── pbix/
│   └── Performance_Analysis_Dashboard.pbix
├── docs/
│   ├── screenshots/    # dashboard images for this README
│   ├── data_dictionary.md
│   └── dax_measures.md
├── reports/
│   └── Performance_Analysis_Dashboard.pdf   # optional exported PDF view
├── .gitignore
├── .gitattributes
└── README.md
```

## Getting Started

1. Clone this repository.
   ```bash
   git clone https://github.com/<your-username>/Performance-Analysis-Dashboard.git
   ```
2. Add your dataset to `data/raw/` (synthetic/anonymized data only if the repo is public).
3. Open `pbix/Performance_Analysis_Dashboard.pbix` in **Power BI Desktop**.
4. Update the data source path/connection if needed (Home → Transform Data → Data Source Settings).
5. Refresh the data and explore.


## Data Privacy

Performance ratings, manager ratings, and PIP status can reflect on individual employees and managers even when aggregated by department. **Do not commit real employee performance data to a public repository.** Use anonymized/synthetic data, or keep the repo private.
