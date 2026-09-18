# Superstore Sales Profitability Analysis

## The main objectives of this project are:

Explore the Superstore sales dataset.
Clean and prepare the data for analysis.
Identify profitability patterns across products and customers.
Segment transactions using K-Means Clustering.
Build a Linear Regression model to explain Profit.
Develop an interactive dashboard for business users.

## How to run this project
**Step 1 -- Clone the repository:**
```bash
git clone https://github.com/Arnoldzzz21/Superstore-Project.git
cd Superstore-Project
```
**Step 2 -- Install dependencies:**
```bash
pip install -r requirements.txt
```
**Step 3 -- Open the notebook:**
```bash
jupyter notebook "Project Superstore.ipynb"
```

Project Workflow

1. Data Preparation
Loaded the dataset
Inspected data quality
Checked missing values
Removed duplicates
Prepared variables for analysis

2. Exploratory Data Analysis (EDA)

Several visualizations were created to understand:

Sales distribution
Profit distribution
Discount impact
Product category performance
Regional performance
Variable correlations

3. Customer Segmentation

K-Means Clustering was applied to group transactions according to purchasing behavior.

The clustering process (K=4) identified four segments:

Mid-Size Orders -- moderate sales and discount levels, solid average profit.
Small Everyday Orders -- the largest group by transaction count, lower average sales, still profitable.
Bulk-Quantity Orders -- a distinct cluster (~1,637 transactions) that is just as profitable as Mid-Size Orders, showing that buying in volume doesn't hurt margin when discounts stay moderate.
Discount Trap -- the only loss-making segment (~9% of orders, ~71% average discount).

4. Linear Regression

A Linear Regression model was developed to predict Profit using:

Sales
Quantity
Discount

The model helps explain how each variable contributes to business profitability.

5. Model Evaluation

The regression model was evaluated using:

R² Score
Mean Absolute Error (MAE)
Regression Coefficients

Although the model explains approximately 27.3% of Profit variability, it provides valuable business insights regarding the impact of discounts and sales on profitability.

Business Recommendations

Based on the analysis, the following recommendations are proposed:

Reduce excessive discounts on low-performing products -- discounts are strongly associated with reduced profitability, though this is a correlational finding, not a proven causal effect.
Review pricing strategies for unprofitable product categories.
Focus marketing efforts on profitable customer segments.
Use customer segmentation to personalize promotional campaigns.
Validate any discount-reduction plan with an A/B test before rolling it out, since simulated profit gains are estimates based on historical correlations, not guarantees.
Include additional business variables in future predictive models to improve accuracy.

Conclusion

This project demonstrates how data analytics and machine learning can support business decision-making by identifying profitability drivers, customer segments, and pricing opportunities. While the Linear Regression model has limited predictive power, it successfully highlights the variables that most influence profit and provides actionable insights for improving overall business performance.

The insights obtained are later presented in an interactive dashboard to support business decision-making.
## Live Dashboard
View it here: https://arnoldzzz21.github.io/Superstore-Project/dashboardsuperstore.html
