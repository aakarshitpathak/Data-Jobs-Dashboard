# 📊 Data Jobs Dashboard

An interactive Power BI dashboard analyzing global data job postings — covering salary trends, remote work patterns, top hiring platforms, and role-specific insights for Data Analyst, Data Scientist, and Data Engineer roles.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/status-complete-brightgreen)

---

## 🔍 Overview

This project explores the global data job market to understand where the opportunities are, what they pay, and what they require — using an interactive two-page Power BI report with drill-through navigation.

**Pages:**
1. **Data Jobs Dashboard** — high-level overview of job postings, salary trends, and top-paying roles
2. **Job Title Drill Through** — role-specific deep dive (salary, work-from-home %, benefits, top platforms, and global distribution)

---

## ✨ Key Features

- 📈 **Job posting trend** over 2024, by month
- 💰 **Highest paying data jobs**, ranked by average yearly salary
- 🔵 **Hourly vs. yearly salary** comparison (scatter chart)
- 🌍 **Global map** of job postings by country
- 🍩 **Work-from-home %, Health Insurance %, and No-Degree-Mention %** by role
- 🌡️ **Gauges** for hourly and yearly salary benchmarks
- 🧩 **Treemap** of data job types (Analyst, Scientist, Engineer, etc.)
- 🏢 **Top hiring platforms** (LinkedIn, Indeed, etc.)
- 🖱️ **Drill-through** from the main dashboard into a role-specific detail page
- 🎛️ **Slicers** for interactive filtering

---

## 🖼️ Preview

```
/Screenshots
  ├── dashboard-overview.png
  └── job-title-drillthrough.png
```

---

## 🗂️ Data Model

| Table | Description |
|---|---|
| `job_postings_flat` | Core fact table — one row per job posting (title, company, salary, location, platform, remote flag, benefits, posted date, etc.) |
| `Waterfall_data` | Supporting table used for waterfall-style breakdowns |
| `funnel_data` | Supporting table used for funnel visuals |

**Key fields used across visuals:** `job_title_short`, `job_country`, `job_via` (posting platform), `job_schedule_type`, `job_work_from_home`, `salary_hour_avg`, `salary_year_avg`, `job_posted_date` (Year/Quarter/Month/Day hierarchy), plus a custom `Salary Star Rating` measure.

> 📁 Dataset: this project uses a "job_postings_flat.csv" style dataset (https://www.kaggle.com/datasets/wandererfakeer/data-jobs-by-lukebarousse)).

---

## 🛠️ Tools & Skills Used

- **Power BI Desktop** — data modeling, DAX measures, report design
- **DAX** — calculated measures (e.g., average salary, star rating, non-null counts)
- **Data visualization** — line, bar, scatter, donut, gauge, treemap, map, pivot table
- **UX design** — drill-through pages, slicers, action buttons for navigation

---

## 🚀 How to Use

1. Clone this repo:
   ```bash
   git clone https://github.com/aakarshitpathak/<your-repo-name>.git
   ```
2. Open `Data_Jobs_Dashboard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).
3. Explore the **Data Jobs Dashboard** page, then right-click a job title bar and select **Drill through → Job Title Drill Through** for role-level details.

---

## 📌 Insights (fill in with your findings)

- Highest paying data role: `__90k USD_`
- % of postings offering remote work: `__10%_`
- Top hiring platform: `_Linkdin__`
- Most in-demand data job title: `_Data Engineer__`

---

## 👤 Author

**Aakarshit Pathak**
- GitHub: [@aakarshitpathak](https://github.com/aakarshitpathak)
- LinkedIn: [aakarshit-p](https://linkedin.com/in/aakarshit-p-501605264)
- Kaggle: [aakarshitpathak](https://kaggle.com/aakarshitpathak)
- Blog: [free28716.wordpress.com](https://free28716.wordpress.com)

---

## 📄 License

This project is open source. Feel free to fork and build on it — attribution appreciated.
