# Cinema Audience Forecasting Project

## 🎯 Project Objective
The primary goal of this project is to forecast the number of visitors to movie theaters for specific future dates. By accurately predicting audience numbers, theaters can optimize their operations, including staffing, inventory management, and resource allocation.

## 🚀 Approach & Workflow
The project follows a structured data science lifecycle:

1. **Data Loading & Integration**: Loading multiple datasets (visits, bookings, theater info) and merging them into a single analytical dataset.
2. **Extended Exploratory Data Analysis (EDA)**: Visualizing data trends, including 7-day rolling averages, monthly seasonality, and feature correlations.
3. **Feature Engineering**: Extracting temporal features (Month, Day) and historical lag features to capture past attendance patterns.
4. **Preprocessing**: Utilizing `Scikit-Learn Pipelines` to automate numerical scaling and categorical encoding.
5. **Model Comparison**: Evaluating four distinct models to find the best fit:
    * Ridge Regression
    * Random Forest
    * XGBoost
    * **LightGBM**
6. **Hyperparameter Tuning**: Optimizing the top-performing model using `RandomizedSearchCV`.
7. **Final Submission**: Generating final predictions and saving them to `submission.csv`.

## 🛠️ Tech Stack
* **Language**: Python
* **Libraries**: 
    * Data Handling: `pandas`, `numpy`
    * Visualization: `matplotlib`, `seaborn`
    * Machine Learning: `scikit-learn`, `xgboost`, `lightgbm`

## 📊 Key Insights from Notebook
* **Seasonality**: The analysis identifies clear patterns based on the day of the week and month.
* **Rolling Averages**: 7-day windows were used to smooth out daily noise and identify long-term trends.
* **Automation**: The use of `Pipeline` ensures that the preprocessing steps are reproducible and leak-proof.

## 📂 File Structure
* `23f2004225-notebook-t32025.ipynb`: The main Jupyter Notebook containing all code and analysis.
* `submission.csv`: Output file containing the final forecasted audience counts.

## ⚙️ How to Run
1. Clone this repository.
2. Ensure you have the datasets in the correct path (as defined by `BASE_PATH` in the notebook).
3. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm
