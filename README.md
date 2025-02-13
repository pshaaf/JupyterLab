# Fannie Mae Loan Default Probability Model

This repository contains a Jupyter Notebook and accompanying code to **predict default probabilities** for a Fannie Mae residential mortgage portfolio. It demonstrates a full end-to-end machine learning workflow—from **data loading** and **feature engineering** to **model training**, **hyperparameter tuning**, and **evaluation**.

## Key Features
- **Data Preprocessing & Imputation**  
  Handles large datasets with missing values, using both numerical (mean/zero) and categorical (custom) imputers.
- **Feature Engineering**  
  Creates new features (e.g., log-transformed house values, interaction terms) and encodes categorical variables (dummy or ordinal).
- **Multiple Model Architectures**  
  Experiments with:
  - Logistic Regression
  - Decision Trees
  - Random Forests
  - XGBoost (boosted trees)
  - Neural Networks (MLPClassifier)
- **Model Evaluation**  
  Uses **Brier Score** and a custom **Skill Score** (compares the model to a naive baseline). Also includes ROC curves and calibration plots for deeper insight.

## Getting Started
1. **Clone or Download** this repository.  
2. **Install Dependencies**  
   - Python 3.7+  
   - Required libraries listed at the top of the notebook (NumPy, Pandas, Scikit-learn, XGBoost, etc.).  
3. **Run the Notebook**  
   - Open the Jupyter Notebook (`.ipynb` file) in your environment.
   - Configure parameters (e.g., sample size, hyperparameters) as desired.
   - Execute cells to clean, transform, and model the data.

## Data Source
- **Fannie Mae Single-Family Loan Performance Data**  
  Publicly available at:  
  [Fannie Mae Data](https://www.fanniemae.com/portal/funding-the-market/data/loan-performance-data.html)  
  (Note: The dataset is large; a sample subset is often used for demonstration.)

## Project Structure
- **`Notebook.ipynb`** (example name)  
  Main Jupyter Notebook performing data preparation, feature engineering, model training, and evaluation.
- **Utility Modules** (if present)  
  Custom Python classes/functions for imputation, scoring, etc.
- **Output**  
  Logs, trained models, or CSV files containing predictions and evaluation metrics.

## Contributing
Feel free to open issues or submit pull requests for improvements, bug fixes, or new modeling approaches.

## License
This project is provided for **educational purposes**. Please review any included license details to ensure compliance with data usage and distribution guidelines.
