# Covid-19 Insights & Global Analysis Dashboard

> **Leveraging Historical Covid-19 Metrics in Power BI to Inform Future Health Interventions**

---

## Executive Summary
This repository features an interactive **Power BI Business Intelligence solution** designed to analyze global COVID-19 pandemic trends, mortality rates, regional distributions, and case evolutions. The dashboard converts raw operational datasets into actionable insights for health data analysis and strategic decision-making.

---

## Core Report Pages & Visuals

### Executive Summary
* **Global Case Status Breakdown:** Donut visual categorizing Active Cases, Total Recoveries, and Total Deaths.
* **Top 10 Countries:** Horizontal bar chart highlighting nations with the highest total confirmed cases.
* **Geographic Spread:** Dynamic map visual showing regional case density and geographic impact.

### Global Trends & Evolution
* **WHO Region Distribution:** 100% Stacked bar chart analyzing recovery-to-confirmed ratios across WHO regions.
* **Epidemic Progression:** Time-series line chart tracking **Daily New Cases** against **Daily New Recoveries**.
* **Interactive Slicers:** Timeline and region filters for dynamic trend analysis.

### Advanced Analysis
* **Key Metrics & KPIs:** High-impact cards displaying **397M Active Cases**, **5.24% Mortality Rate**, **713K Total Deaths**, and **268M Total Tests**.
* **Monthly Distribution:** Pie visual breaking down total recoveries and deaths across calendar months.
* **Regional Breakdown:** Comparative bar visuals isolating cases by geographic zone.

---

## Data Architecture & DAX Measures

### Relational Tables
* `country_wise_latest`
* `day_wise`
* `full_grouped`
* `usa_county_wise`
* `worldometer_data`

### Core DAX Calculations

```dax
// Mortality Rate Calculation
Mortality Rate = 
DIVIDE(
    SUM('country_wise_latest'[Total Deaths]),
    SUM('country_wise_latest'[Total Confirmed]),
    0
)

// Total Active Cases Measure
Total Active Cases = 
SUM('country_wise_latest'[Active])
```


## Contact

Name: Anicet Baraka CIza

LinkedIn: https://www.linkedin.com/in/anicetbarakaciza/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BecQzM0I%2BRMO6dL%2BQo38lmw%3D%3D

GitHub: [Anicet Baraka Ciza] (https://github.com/iamanicet)

Email: cizaanicetbaraka@gmail.com

