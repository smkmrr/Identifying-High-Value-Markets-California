# Identifying High-Value Real Estate Markets
**Author:** [Your Name]

## Business Objective
A real estate investment firm seeks to expand into the California market, focusing exclusively on premium, high-value neighborhoods (the top 20% of the market). However, in rapidly developing areas, exact median house prices are often missing or unreliable. 

This project builds a machine learning pipeline capable of identifying whether a neighborhood belongs to the "High-Value" tier based solely on its geographic coordinates, demographics, and local infrastructure, providing an automated tool for initial market screening.

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
* **Techniques:** Binary Classification, Unsupervised Learning (K-Means Clustering), Hyperparameter Tuning (GridSearchCV), Data Pipeline Engineering

## Key Findings & Results
1. **Market Segmentation:** Using K-Means clustering, the algorithm naturally identified three distinct types of neighborhoods, isolating high-density, newer developments from older, established regions based purely on demographics.
2. **Predictive Performance:** The optimized Random Forest classifier achieved a strong balance on unseen test data, prioritizing a reduction in wasted operational resources.
   * **F1-Score:** 0.7776
   * **Precision:** 86.4% (When the model flags a market as high-value, it is highly reliable).
   * **Recall:** 70.7% (The model successfully identified the majority of hidden premium markets).

## Project Structure
* `identifying_high_value_real_estate.ipynb`: The core Jupyter Notebook containing the full EDA, data preprocessing pipelines, model training, and business risk analysis (Confusion Matrix).

## How to Run
To ensure strict reproducibility, a global random seed (`42`) was applied throughout the pipeline. 

1. Clone this repository to your local machine.
2. Create and activate a virtual environment (recommended).
3. Install the required execution and data science libraries:
   `pip install ipykernel pandas numpy scikit-learn matplotlib seaborn`
4. Select your virtual environment as the kernel and run the `identifying_high_value_real_estate.ipynb` notebook from top to bottom.