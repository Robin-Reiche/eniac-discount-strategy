# Eniac Discount Strategy Analysis

A data analysis project examining the effectiveness of discount strategies for Eniac, a tech retailer. This project analyzes sales data to determine whether discounts increase or decrease overall revenue.

## Project Overview

Eniac's board is debating whether to continue offering discounts. Some believe discounts drive sales, while others think they reduce revenue without increasing customer loyalty. This analysis uses real sales data to provide data-driven insights.

## Key Findings

- **Black Week Performance**: Revenue per day was significantly higher during Black Week compared to non-promotional periods
- **Discount Impact**: Moderate discounts (~20-25%) proved most effective
- **Customer Behavior**: Higher basket values and multi-product orders during promotional periods
- **Recommendation**: Continue strategic discounts during key marketing events (Black Friday, Christmas)

## Project Structure

```
eniac-discount-strategy/
├── notebooks/
│   ├── 01_explore_brands.ipynb      # Brand data exploration
│   ├── 02_explore_orders.ipynb      # Orders data exploration
│   ├── 03_explore_orderlines.ipynb  # Order lines exploration
│   ├── 04_explore_products.ipynb    # Products data exploration
│   ├── 05_merge_dataframes.ipynb    # Data merging pipeline
│   ├── 06_price_pattern_analysis.ipynb    # Pattern discovery
│   ├── 07_fix_price_formats.ipynb   # Price format cleaning
│   └── 08_discount_analysis.ipynb   # Final discount analysis
├── data/
│   ├── raw/                         # Original CSV files
│   └── processed/                   # Cleaned/merged datasets
├── docs/
│   └── case_study.pdf               # Original case study document
├── requirements.txt
└── README.md
```

## Data Pipeline

1. **Exploration** (Notebooks 01-04): Analyze each data source independently
2. **Merging** (Notebook 05): Combine brands, orders, orderlines, and products
3. **Pattern Analysis** (Notebook 06): Discover price format issues (European number formats with dots as thousand separators)
4. **Cleaning** (Notebook 07): Fix price formats based on pattern analysis
5. **Discount Analysis** (Notebook 08): Final discount effectiveness analysis

## Technologies Used

- Python 3.11
- pandas - Data manipulation
- seaborn - Statistical visualizations
- matplotlib - Plotting

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/linkedIn_profile.git

# Navigate to project
cd linkedIn_profile/data/projects/group_projects/eniac-discount-strategy

# Install dependencies
pip install -r requirements.txt
```

## Usage

Run the notebooks in numerical order (01-08) to reproduce the analysis:

```bash
jupyter notebook notebooks/
```

## Data Description

| File | Description | Rows |
|------|-------------|------|
| brands.csv | Brand information | - |
| orders.csv | Order transactions | ~227K |
| orderlines.csv | Individual order items | ~293K |
| products.csv | Product catalog | - |

## Author

Robin Reiche - Data Science Portfolio Project

## License

This project is for educational and portfolio purposes.
