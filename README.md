<p align="center">
  <img src="banner.png" alt="Brazilian E-Commerce Data Analysis Banner" width="100%">
</p>

# Brazilian E-Commerce Data Analysis (Olist)

Exploratory data analysis of the Brazilian Olist e-commerce dataset using Python, Pandas, NumPy, and Matplotlib.

The goal is to understand sales trends, product categories, customer locations, delivery performance, and customer reviews through data cleaning, analysis, visualization, and interpretation.

## Project Objectives

- Analyze monthly order volume and GMV trends.
- Identify product categories with the highest GMV.
- Explore GMV by customer state.
- Analyze delivery duration and delivery punctuality.
- Examine customer review scores and their relationship with delivery status.
- Calculate metrics from the dataset instead of manually entering results.

## Technologies

- Python 3
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib

## Project Structure

Place the Olist CSV files inside `data/raw/`.

```text
olist-analysis/
├── data/
│   └── raw/
│       ├── olist_orders_dataset.csv
│       ├── olist_order_items_dataset.csv
│       ├── olist_products_dataset.csv
│       ├── olist_customers_dataset.csv
│       ├── olist_order_payments_dataset.csv
│       ├── olist_order_reviews_dataset.csv
│       └── olist_sellers_dataset.csv
├── olist_analysis_final.ipynb
├── outputs/
│   └── figures/
└── README.md
```

Keep the notebook filename consistent with the actual file in your repository. If your notebook has a different name, update the filename above.

## Installation and Usage

### 1. Install the dependencies

Make sure Python 3 is installed, then run:

```bash
pip install pandas numpy matplotlib jupyter
```

### 2. Add the dataset

Download the Olist dataset and place the required CSV files in `data/raw/`.

### 3. Start Jupyter Notebook

From the project directory, run:

```bash
jupyter notebook
```

Open `olist_analysis_final.ipynb` and execute the notebook from top to bottom using **Run All**.

> Note: The notebook must be run with the dataset available. Report final metrics only after checking the actual output.

## Analysis and Visualizations

The notebook is designed to produce eight visualizations:

1. **Monthly Order Trend** — changes in order volume over time.
2. **Monthly GMV Trend** — changes in the value of items sold over time.
3. **Top Product Categories by GMV** — categories contributing the most item value.
4. **Top Customer States by GMV** — customer states associated with the highest GMV.
5. **Delivery-Time Distribution** — distribution of delivery duration for orders with usable delivery dates.
6. **On-Time vs. Late Delivery** — comparison of actual delivery dates with estimated delivery dates.
7. **Review-Score Distribution** — distribution of customer review scores.
8. **Review Scores by Delivery Status** — comparison of review scores for on-time and late deliveries.

## Key Metrics

Depending on the fields available and the definitions used in the notebook, the analysis can calculate:

- Total number of orders
- Gross Merchandise Value (GMV)
- Freight value
- Average order value (AOV)
- Average and median delivery duration
- On-time and late delivery rates
- Average review score by delivery status
- Repeat-purchase rate, if customer identifiers support the calculation

**Metric definitions matter.** Missing delivery dates should not automatically be counted as on-time deliveries. Orders without usable delivery timestamps should be handled explicitly in delivery-time and punctuality calculations.

## Interpretation Notes

- GMV represents the value of items sold; it is not company profit.
- The state visualization represents GMV by customer state, not an overall measure of state performance.
- Correlation indicates association, not causation. Any reported correlation must be calculated from the dataset and identify the variables being compared.
- Business recommendations should follow from the notebook's actual results. Suggested targets should be labelled as proposals, not measured outcomes.

## Results

Run the notebook to generate the actual metrics and charts. Add exported figures or screenshots here only after creating them. Avoid publishing specific KPI values until they have been checked against the executed notebook.

## Possible Business Recommendations

Based on the findings produced by the analysis, recommendations may include:

- Investigating product categories that contribute strongly to GMV.
- Identifying periods or customer states where delivery delays are more frequent.
- Monitoring customer reviews alongside delivery performance.
- Using monthly order and GMV trends to support planning.

Keep only recommendations supported by the results.

## Author

- **Name:** Yahya Charih
- **GitHub:** https://github.com/charihyahya-max
- **Project Repository:** https://github.com/charihyahya-max/olist-ecommerce-analytics.git

Replace the placeholders above with your own information.

---

*Educational portfolio project. Results depend on the dataset version and the metric definitions used in the notebook.*
