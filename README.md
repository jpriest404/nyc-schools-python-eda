# Standardized Testing & Demographic Exploratory Data Analysis (Python)

## 📊 Executive Summary
An exploratory data analysis (EDA) conducted in **Python (`pandas`, `numpy`)** examining standardized SAT performance across New York City public schools. This analysis identifies top-performing academic institutions in mathematics, evaluates total combined score distributions across all five boroughs, and calculates borough-level variance and standard deviation to measure performance consistency.

## 🎯 Analytical Objectives
1. **Top Math Performance Identification:** Filter schools achieving exceptional quantitative scores (>=80% or >=640 out of 800 math score).
2. **Composite Score Ranking:** Engineer a composite `total_SAT` metric across math, reading, and writing sections to isolate the top 10 performing schools citywide.
3. **Borough-Level Statistical Dispersion:** Group schools by `borough` and apply `.agg()` to compute school counts, mean `total_SAT`, and standard deviation (`std`) to identify which borough exhibits the widest performance gap.

## 🛠️ Python Toolkit & Methods
* **Data Manipulation (`pandas`):** Boolean indexing, column engineering, multi-column sorting (`.sort_values()`), and grouped aggregations (`.groupby().agg()`).
* **Statistical Analysis (`numpy`):** Mean, standard deviation, and rounding transformations to quantify score variability across demographic regions.

## 📂 Repository Structure
* `notebooks/nyc_schools_eda.ipynb` — Jupyter notebook containing data loading, cleaning, and statistical EDA.

## 💡 Key Findings & Insights
* **Top Math Performers:** Specialized magnet campuses lead the district in quantitative performance, led by **Stuyvesant High School (754 avg math)**, **Bronx High School of Science (714)**, and **Staten Island Technical High School (711)**.
* **Top Composite SAT Rankings:** When evaluating total combined scores (`total_SAT`), **Stuyvesant High School** leads the district with a composite score of **2144**, followed by **Bronx Science (2041)** and **Staten Island Tech (2041)**.
* **Borough Variance:** **Manhattan** exhibits the largest standard deviation in composite SAT scores, indicating the widest disparity between specialized institutions and general neighborhood campuses within a single borough.
