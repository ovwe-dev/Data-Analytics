# Healthcare Operations \& Billing Intelligence Analysis

## Project Title

**Healthcare Operations \& Billing Intelligence Analysis**

## Business Problem

Healthcare organisations need to understand patient demand, cost, admission patterns, bed utilisation, payer mix and test-result activity so they can make better operational and financial decisions.

This project uses Python to answer questions such as:

* Which medical conditions generate the most admissions?
* Which conditions generate the highest total billing?
* Which admission types have the highest average billing?
* How long do patients stay?
* How do admissions change over time?
* Which insurance providers account for the most billing?
* How do test results vary by medical condition?

## Dataset Used

`healthcare\_dataset.csv`

The dataset contains **10,000 rows and 15 original columns** of synthetic healthcare data, including patient demographics, medical condition, admission and discharge dates, hospital, insurance provider, billing amount, admission type, medication and test result.

> This dataset is synthetic and is used for learning and portfolio purposes, not clinical decision-making.

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Key Analysis Completed

* Data inspection using `df.head()`, `df.shape`, `df.info()`, `df.describe()` and `df.isnull().sum()`
* Duplicate-row checks
* Data-type validation
* Date conversion
* Text-format standardisation
* Feature engineering:

  * `Length\_of\_Stay`
  * `Admission\_Month`
  * `Admission\_Quarter`
  * `Age\_Group`
* GroupBy analysis of conditions, admission types, insurers and hospitals
* Required visualisations:

  * Admissions by Medical Condition
  * Total Billing by Medical Condition
  * Average Billing by Admission Type
  * Length of Stay Distribution
  * Monthly Admission Trend
  * Test Results by Medical Condition
* Additional insurer, age-group and billing-driver analysis

## Main Insights

* **Asthma** has the highest admission count: **1,708**.
* **Cancer** has the highest total billing: approximately **43.49 million**.
* **Urgent** admissions have the highest average bill: approximately **25,960.83**.
* **Emergency** admissions have the longest average stay: approximately **15.61 days**.
* **Cigna** has the highest total billing among insurers: approximately **52.34 million**.
* **October 2022** has the highest monthly admission count: **207**.
* There are **3,456 abnormal test results**, the largest test-result category.
* Length of stay has almost no linear relationship with billing in this synthetic dataset, with a correlation of approximately **-0.014**.

## Recommendations

1. Report patient volume and financial value as separate KPIs.
2. Investigate the service mix behind higher average Urgent-admission billing.
3. Monitor length of stay by admission pathway for bed-capacity planning.
4. Strengthen payer dashboards for high-value insurers such as Cigna and Aetna.
5. Use monthly admission trends for workforce and capacity planning.
6. Monitor abnormal/inconclusive test-result follow-up workload where operational data is available.
7. Standardise hospital master data before hospital benchmarking.
8. Use multivariable analysis to identify billing drivers rather than relying on length of stay alone.

## Repository Structure

```text
healthcare-analysis/
├── healthcare\_analysis.ipynb
├── healthcare\_dataset.csv
├── README.md
└── LinkedIn\_Post.md
```

## Portfolio Note

This project was completed as a Data Analyst / Business Intelligence portfolio exercise. The emphasis is on explaining analytical choices, interpreting results and translating data into business recommendations.

