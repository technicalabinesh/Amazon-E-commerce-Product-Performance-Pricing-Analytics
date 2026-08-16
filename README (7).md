# Amazon E-commerce Product Performance & Pricing Analytics

## Project Overview

This project analyzes Amazon e-commerce product data to understand **product performance, customer engagement, pricing, discounts, promotions, and product visibility**.

The notebook works with an uncleaned Amazon product dataset and uses Python-based data analysis and visualization to transform the raw data into an analysis-ready dataset and generate insights.

### Project Goal

The analysis focuses on:

- Product ratings and review counts
- Monthly purchase activity
- Current/discounted pricing and listed pricing
- Best Seller status
- Sponsored vs. organic visibility
- Coupon availability
- Buy Box availability
- Delivery information
- Sustainability badges

## Dataset

The notebook reports an initial dataset size of **42,675 rows and 13 columns**.

### Columns

| Column | Description |
|---|---|
| `title` | Product title |
| `rating` | Product rating |
| `number_of_reviews` | Number of customer reviews |
| `bought_in_last_month` | Approximate number of purchases in the past month |
| `current_discounted_price` | Current/discounted product price |
| `price_on_variant` | Price information associated with the selected variant |
| `listed_price` | Listed/original price information |
| `is_best_seller` | Best Seller badge information |
| `is_sponsored` | Sponsored or organic listing |
| `is_couponed` | Coupon availability |
| `buy_box_availability` | Buy Box/cart availability |
| `delivery_details` | Delivery information |
| `sustainability_badges` | Sustainability/business badges |

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook / Google Colab

## Analysis Workflow

The notebook includes the following major stages:

1. **Data Understanding**
   - Inspect dataset shape
   - Review column names and data types
   - Generate descriptive summaries
   - Examine missing values

2. **Data Cleaning**
   - Standardize column names
   - Remove duplicate rows
   - Analyze missing-value percentages
   - Prepare fields for further analysis

3. **Exploratory Data Analysis**
   - Analyze product ratings and reviews
   - Study purchase activity
   - Explore pricing and discounts
   - Compare sponsored and organic products
   - Examine Best Seller and coupon-related patterns

4. **Visualization**
   - Use Matplotlib and Seaborn for statistical/analytical plots
   - Use Plotly for interactive visual exploration

## Data Quality Findings

The raw dataset contains substantial duplication and missing values.

- Initial rows: **42,675**
- Duplicate rows removed: **32,602**
- Rows after duplicate removal: **10,073**
- `sustainability_badges` has the highest missing-value percentage at approximately **91.43%**
- `buy_box_availability` has approximately **34.49%** missing values
- `delivery_details` has approximately **29.16%** missing values
- `current_discounted_price` has approximately **29.13%** missing values

These findings make data cleaning an important part of the project.

## Example Data

The dataset contains products such as wireless microphones, USB charging cables, Apple AirPods, and Apple AirTags, along with their ratings, reviews, purchase indicators, prices, badges, and promotional information.

## Repository Structure

```text
.
├── Amazon_E_commerce_Product_Performance_&_Pricing_Analytics.ipynb
├── amazon_sales_data_uncleaned.csv
└── README.md
```

> Place the CSV file in the same directory as the notebook, or update the `FILE_PATH` variable in the notebook.

## How to Run

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <YOUR_REPOSITORY_NAME>
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

### 3. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Amazon_E_commerce_Product_Performance_&_Pricing_Analytics.ipynb
```

### 4. Dataset Path

The notebook reads the source CSV using a configurable `FILE_PATH`.

Update it according to your local environment, for example:

```python
FILE_PATH = "amazon_sales_data_uncleaned.csv"
```

## Key Project Highlights

- Real-world style e-commerce dataset
- 42K+ raw product records
- Extensive duplicate removal and data-quality analysis
- Missing-value profiling
- Price and promotion analysis
- Product popularity analysis
- Best Seller and sponsored-product analysis
- Interactive Plotly visualization
- Python-based end-to-end exploratory data analysis

## Skills Demonstrated

**Data Analytics:** Data cleaning, EDA, missing-value analysis, duplicate detection, descriptive statistics

**Python:** Pandas, NumPy, Matplotlib, Seaborn, Plotly

**Business Analysis:** Product performance, pricing, promotions, customer engagement, visibility

**Visualization:** Statistical charts and interactive Plotly visualizations

## Author

**Abinesh M.**

B.Tech – Artificial Intelligence & Data Science

---

If you find this project useful, consider giving the repository a ⭐.
