The aim of this project was to determine the optimal prices that maximize revenue and profit
for several retail products. For this purpose, demand models were obtained by fitting linear
models (Ordinary Least Squares and Poisson) that predict demand at different historical prices.
The models were then used to obtain revenue and profit functions which were differentiated
to obtain the optimal price that maximizes both metrics. Prices were considered for the
maximization of both revenue and profit because both can be business objectives depending
on the situation (e.g., revenue is more important than profit for initial market penetration and
growth). 


# Price Optimization using Generalized Linear Models (R)

## Overview
Data science project focused on optimizing product pricing to maximize **revenue and profit** using demand modeling and mathematical optimization.

Built a pricing engine that estimates **price elasticity of demand** across multiple products and identifies optimal price points using **OLS and Generalized Linear Models (Poisson)**.

The solution translates statistical models into **actionable pricing strategies** for commercial decision-making.

---

## Business Problem
Companies often set prices based on intuition or static rules, leading to:

- Overpricing → reduced demand and lost revenue  
- Underpricing → missed profit opportunities  
- Lack of visibility into price-demand relationships  

There is a need for a **data-driven approach** to determine optimal pricing strategies.

---

## Solution
A pricing optimization framework was developed to:

- Model demand as a function of price  
- Estimate **price elasticity** across products  
- Construct **revenue and profit functions**  
- Identify optimal price points through mathematical optimization  
- Compare different modeling approaches (OLS vs GLM)  

The system is designed to be **scalable and reusable** across datasets.

---

## Methodology

### 1. Data Exploration
- Exploratory analysis on price and demand  
- Computation of **coefficient of variation (CV)** to identify products with sufficient price variability  

### 2. Demand Modeling

Two approaches were implemented:

**OLS (Linear Regression)**  
- Models demand as a linear function of price  
- Interpretable and simple baseline  

**Poisson GLM (Log-link)**  
- Suitable for count data (units sold)  
- Captures non-linear demand behavior  

Model selection based on:
- OLS → R² and coefficient sign  
- GLM → AIC and McFadden Pseudo R²  

---

### 3. Price Optimization

From the demand models, the following functions were derived:

- Revenue = Price × Demand  
- Profit = (Price – Cost) × Demand  

Optimal prices are obtained by maximizing these functions:

- Revenue-maximizing price  
- Profit-maximizing price  

For OLS models, closed-form solutions are used.  
For GLMs, numerical optimization is applied.

---

## Example Output

The model generates demand curves and identifies optimal pricing points:

- Blue curve → Revenue  
- Red curve → Profit  
- Vertical lines → Optimal prices  

---

## Results & Insights

- Optimal prices were consistently **lower than average market prices**, suggesting potential overpricing  
- Price reductions could **increase both demand and total revenue**  
- Different models (OLS vs GLM) yield different optimal strategies, requiring model selection  
- Demonstrates how statistical modeling can directly impact **commercial strategy**

---

## Tech Stack

- R  
- Statistical Modeling  
- Generalized Linear Models (GLM)  
- Regression Analysis  
- Data Visualization (ggplot2)  

---

## Key Techniques

- Demand modeling & price elasticity estimation  
- Model selection using R², AIC, and Pseudo R²  
- Revenue & profit function construction  
- Numerical optimization  
- Automated multi-product analysis  

---


---

## Business Value

This project demonstrates how data science can:

- Replace intuition with **quantitative pricing strategies**  
- Identify **hidden revenue opportunities**  
- Support **pricing decisions at scale**  
- Bridge statistical modeling with real business impact  

---

## Limitations & Next Steps

- Incorporate **customer segmentation** (e.g. clustering)  
- Include **external factors** (seasonality, competition)  
- Extend to **dynamic pricing systems**  
- Validate results with real-world experiments (A/B testing)

---

## Real-World Applications

This approach can be applied to:

- Retail pricing strategy  
- E-commerce dynamic pricing  
- SaaS pricing optimization  
- Promotion and discount analysis  

---

## 🔗 Links

- 🚀 Project Repository  
- 🌐 https://federicogarland.github.io/FedericoGarlandWebsite/  
- 💼 https://www.linkedin.com/in/federico-garland/
