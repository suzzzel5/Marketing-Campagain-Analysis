# Marketing Campaign Analytics Project

End-to-end customer and campaign analysis using Python, with data cleaning, feature engineering, exploratory analysis, and business-focused visual storytelling.

## Project Overview

This project analyzes a retail marketing campaign dataset to answer practical business questions:

- Who are our customers?
- Which campaigns perform best?
- What products drive spending?
- Which channels are preferred?
- What separates responders from non-responders?

The analysis is done in Jupyter notebooks and supported by clear visual insights.

## About the Dataset

- **Source file:** `data/marketing_campaign.csv`
- **Cleaned file:** `data/marketing_campaign_clean.csv`
- **Records:** 1,260 customers
- **Features:** 30 columns (demographics, purchases, campaign behavior, and engineered features)
- **Target column:** `Response` (1 = accepted final campaign offer, 0 = not accepted)

### Main Data Groups

- **Demographics:** `Age`, `Education`, `Marital_Status`, `Income`, `Has_Children`
- **Purchase behavior:** wine, meat, fruit, fish, sweets, gold spending
- **Channel behavior:** web, store, catalog, and deal purchases
- **Campaign response:** `AcceptedCmp1` ... `AcceptedCmp5`, `Response`
- **Engineered features:** `Total_Spend`, `Total_Purchases`, `Total_Campaigns_Accepted`, `Days_Customer`

## What I Did in This Project

### 1) Data Exploration

- Reviewed structure, data types, and distributions
- Checked missing values and suspicious patterns

### 2) Data Cleaning & Transformation

- Handled data quality issues and outliers
- Prepared analysis-ready dataset
- Engineered helpful business features (total spend, purchase totals, campaign acceptance totals, loyalty days)

### 3) EDA & Visualization

- Built simple, readable charts for each key business question
- Added easy-to-understand insight notes below every figure
- Compared responders vs non-responders across behavior dimensions

### 4) Business Interpretation

- Converted chart findings into direct campaign recommendations
- Highlighted which segments and channels to prioritize

## Key Headline Metrics

- **Final campaign response rate:** 11.19%
- **Median age:** 53 years
- **Median income:** $38,815.5
- **Average total spend:** $240.02

## Notebooks

- `notebooks/01_data_exploration.ipynb` - Initial understanding and profiling
- `notebooks/02_data_cleaning_transformation.ipynb` - Cleaning, corrections, and feature creation
- `notebooks/03_eda_visualizations.ipynb` - Final visual analysis with insights

## Visual Gallery (All Figures)

### Data Quality / Preparation

#### Outlier Check After Corrections
![Outlier Check](Figures/Outlier%20check%20after%20year_birth%20and%20income%20correction.png)

### Customer Profile

#### Who Is Our Customer?
![Who is our customers](Figures/Who%20is%20our%20customers.png)

### Campaign Performance

#### Campaigns Accepted Per Customer
![Campaigns accepted per customer](Figures/campagins%20accepted%20per%20customer.png)

#### How Many Campaigns Did Each Customer Accept?
![How many campaigns accepted](Figures/How%20many%20campagins%20did%20each%20customer%20Accepted.png)

### Product Spending

#### Average Spend by Product Category
![Average spend by product category](Figures/Average%20spend%20by%20prouduct%20category.png)

#### Average Spend per Product Category (Alternative)
![Average spend per product catg](Figures/Average%20spend%20per%20product%20catg.png)

### Channel Behavior

#### Customer Purchase Channel
![Customer purchase channel](Figures/customer%20purcahase%20chanel.png)

#### Channel Usage: Responders vs Non-Responders
![Channel usage responders vs non responders](Figures/Channel%20usge%20thorugh%20responders%20vs%20non%20responders.png)

### Responder vs Non-Responder Comparison

#### Total Spend by Response Group
![Total spend responders vs non responders](Figures/Total%20spend%20by%20responders%20and%20non%20responders.png)

#### Responders vs Non-Responders
![Responders vs non-responders](Figures/Responders%20VS%20non-responders.png)

### Loyalty / Tenure

#### Response Rate by Customer Tenure
![Response rate by tenure](Figures/Response%20Rate%20by%20customer%20tenure.png)

## Important Insights

- Most customers do not accept campaigns; a small segment drives most positive responses.
- The final offer performs much better than earlier campaigns.
- Spending is concentrated in a few categories (especially wines).
- Responders show stronger digital behavior (web/catalog/deals).
- Customer segmentation (age, income, behavior, tenure) is essential for better campaign ROI.

## Business Recommendations

- Build segmented campaigns instead of one generic message for all users.
- Prioritize high-value and high-probability responder segments.
- Increase digital-first campaign delivery for likely responders.
- Use recency and tenure triggers for reactivation and retention campaigns.
- Test offers/messages systematically and track uplift by segment.

## Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## How to Run

1. Clone this repository
2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

3. Open notebooks:

```bash
jupyter notebook
```

4. Run notebooks in order:
   - `01_data_exploration.ipynb`
   - `02_data_cleaning_transformation.ipynb`
   - `03_eda_visualizations.ipynb`

## Repository Structure

```text
Marketing Campaign/
├── data/
│   ├── marketing_campaign.csv
│   └── marketing_campaign_clean.csv
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_cleaning_transformation.ipynb
│   └── 03_eda_visualizations.ipynb
├── Figures/
└── README.md
```

## Author

This project demonstrates practical marketing analytics: from raw customer data to campaign-focused business insights.

