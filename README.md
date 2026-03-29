# Does Where You Live Decide How You Spend? Household Expenditure Analysis, Sikkim

A spatial analysis of household expenditure patterns across Sikkim's four districts using NSS 72nd Round data (2014-15), GIS mapping, and statistical analysis.

---

## Key Finding

Household size and domestic service expenditure show a **strong positive correlation of 0.77** across Sikkim's districts. Larger households spend significantly more on domestic services. But when it comes to business services, a clear **rural-urban divide** emerges: urban households invest more in business services as household size grows, while rural households show no such pattern, constrained by geography, infrastructure, and limited economic opportunity.

---

## About This Project

Sikkim, India's smallest state by population, offers a unique lens for studying socio-economic patterns. Its four districts (North, South, East, West) each have distinct geographical and demographic characteristics, making district-level spatial analysis particularly revealing.

This study uses NSS household expenditure data to answer two questions:

1. How does household size correlate with expenditure on domestic services across districts?
2. Is there a rural-urban divide in household expenditure on business services?

**Tools used:** QGIS · Microsoft Excel · NSS Microdata  
**Dataset:** National Sample Survey, 72nd Round (July 2014 - June 2015)  
**Variables:** Household size · Domestic services expenditure (530-533) · Business services expenditure (630-632) · Sector (Rural/Urban)

---

## Maps

![](maps/Domestic-Average-Expenditure.png)
![](maps/Domestic-Average-HouseholdSize.png)
![](maps/Rural-Weighted-Average-Expense.png)
![](maps/Rural-Weighted-Average-HouseholdSize.png)
![](maps/Sikkim-Map-Reprojected.png)
![](maps/StandardDeviation-Domestic-Household-Expense.png)
![](maps/StandardDeviation-Domestic-Household-Size.png)
![](maps/Urban-Average-Weighted-Expense.png)
![](maps/Urban-Average-Weighted-HouseholdSize.png)

---
## What the Maps Show

| District | Household Size | Avg Domestic Expenditure | Pattern |
|---|---|---|---|
| North | Lowest (avg 1) | Lowest deviation | Rugged terrain, protected areas, sparse population |
| East | Highest (avg 3) | Highest deviation | Urban concentration, better connectivity |
| West | Average (avg 2) | Low deviation | Agricultural focus |
| South | Average (avg 2) | Second highest | Mixed urban-rural |

**Rural vs Urban business expenditure:**
- Rural North: lowest weighted expenditure, terrain and infrastructure constraints
- Rural East: highest weighted expenditure, proximity to urban economic activity
- Urban areas: household size positively drives business expenditure
- Rural areas: household size does NOT drive business expenditure, urban dominance limits rural growth

---

## Methodology

- NSS data filtered for Sikkim-specific households
- Statistical summaries: mean, median, standard deviation, correlation (Excel)
- Weighted averages calculated separately for rural and urban setups per district
- District-level shapefiles used to map expenditure and household size patterns
- Classification methods: Standard deviation (deviation maps) and Quantile (average maps)

---

## Policy Implications

The rural-urban divide in business service expenditure points to a structural gap. North and West Sikkim need targeted infrastructure investment to enable rural households to participate in the services economy. East Sikkim's urban model, where larger households actively invest in business services, could serve as a framework for developing rural business ecosystems in other districts. Existing schemes like PM Gram Sadak Yojana and NITI Aayog's North East development framework provide entry points for such interventions.

---

## Limitations

- Sample data had higher rural representation, weighted averages used to compensate
- Findings reflect 2014-15 conditions and are based on a limited sample
- Correlation does not imply causation, other socio-cultural factors may influence patterns
- Urban data availability was limited, which may affect precision of urban-level inferences

---

## Repo Structure

```
Sikkim-Household-Expenditure-GIS/
│
├── report/
│   └── SIKKIM_FINAL.pdf
│
├── maps/
│   ├── Domestic-Average-Expenditure.png
│   ├── Domestic-Average-HouseholdSize.png
│   ├── Rural-Weighted-Average-Expense.png
│   ├── Rural-Weighted-Average-HouseholdSize.png
│   ├── Sikkim-Map-Reprojected.png
│   ├── StandardDeviation-Domestic-Household-Expense.png
│   ├── StandardDeviation-Domestic-Household-Size.png
│   ├── Urban-Average-Weighted-Expense.png
│   └── Urban-Average-Weighted-HouseholdSize.png
│
└── README.md
```

---

## Report

[Click here to view the full report](report/SIKKIM_FINAL.pdf)

---

*Made by Pranav Sharma · BS Analytics and Sustainability Studies · TISS Mumbai · Sem III*
