# Time-Series-Sunspot-Forecasting

## **Overview**
This project aims to predict sunspot activity using time-series forecasting models, with predictions made across three different time units: **daily**, **monthly**, and **yearly**. The goal is to forecast the number of sunspots for future periods based on historical sunspot data. The project leverages **Prophet**, a robust time-series forecasting tool, and handles three different datasets, each focused on a different time unit:
- **Daily data**: Prediction for 100, 200, and 365 days into the future.
- **Monthly data**: Prediction for 1, 6, and 9 months into the future.
- **Yearly data**: Prediction for 1, 10, and 20 years into the future.

## **Project Workflow**
1. **Data Preprocessing**:
   - Handling missing values and preparing the data for Prophet by transforming it into the required format (columns `ds` for date and `y` for sunspot count).
   - Processing three different time-series datasets:
     - **Daily data**: Observations made every day.
     - **Monthly data**: Observations aggregated by month.
     - **Yearly data**: Observations aggregated by year.

2. **Exploratory Data Analysis (EDA)**:
   - Visualizing trends and patterns in sunspot activity over different time scales (daily, monthly, yearly).
   - Identifying seasonality and cyclical behavior in the data.

3. **Model Training**:
   - Training three different Prophet models on each dataset:
     - **Linear Growth**: For a straight-line trend.
     - **Logistic Growth**: For trends that are capped.
     - **Flat Growth**: For constant trends.

4. **Model Evaluation**:
   - Evaluating models by comparing forecasts with historical data.
   - Identifying the best-performing model for each dataset.

5. **Prediction**:
   - Predicting sunspot activity for different future time periods based on the dataset:
     - **Daily data**: Predictions for 100, 200, and 365 days.
     - **Monthly data**: Predictions for 1, 6, and 9 months.
     - **Yearly data**: Predictions for 1, 10, and 20 years.

6. **Results Visualization**:
   - Visualizing predictions against actual sunspot data for different time units to compare accuracy and forecast trends.

## **Key Features Analyzed**
- **Daily Sunspot Data**: Analysis of sunspot activity on a daily basis.
- **Monthly Sunspot Data**: Analysis of sunspot activity aggregated by month.
- **Yearly Sunspot Data**: Analysis of sunspot activity aggregated by year.
- **Growth Models**: Comparing linear, logistic, and flat growth models for each dataset.
- **Time Horizons**: Forecasting for different periods based on daily, monthly, and yearly time units.

## **Results**
- **Daily Predictions**: Forecast for 100, 200, and 365 days into the future, with a comparison of model performance.
- **Monthly Predictions**: Forecast for 1, 6, and 9 months, with an evaluation of each model's accuracy.
- **Yearly Predictions**: Forecast for 1, 10, and 20 years, with the comparison of forecast results across models.
- **Visualization**: Each forecast is visualized and compared to actual data for validation.

## **Tools and Technologies**
- **Programming Language**: Python
- **Time-Series Forecasting**: Prophet
- **Data Analysis & Preprocessing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Notebook Environment**: Jupyter Notebook

## **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/drashti-sanghani/Time-Series-Sunspot-Forecasting.git
   
2. Navigate into the project directory:
   ```bash
   cd time-series-sunspot-forecasting

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt

4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook

## **Dataset**
The project uses three different datasets:
- **Daily Sunspot Data:** The dataset contains daily observations of sunspot activity.
- **Monthly Sunspot Data:** The dataset aggregates sunspot data on a monthly basis.
- **Yearly Sunspot Data:** The dataset aggregates sunspot data on a yearly basis.

The data is available in three separate CSV files: SN_d_tot_V2.0.csv, SN_m_tot_V2.0.csv, and SN_y_tot_V2.0.csv.

## **Acknowledgement**
- **Prophet:** For providing a robust and easy-to-use forecasting tool.
- **Pandas, NumPy, Matplotlib, Seaborn:** For their contributions to data analysis and visualization in Python.
- **Data Sources:** The dataset was sourced from publicly available sunspot data archives.

## **Future Work**
- **Incorporating External Variables:** Future work could integrate additional variables, such as solar activity indicators or space weather data, to improve the accuracy of predictions.
- **Real-Time Predictions:** Extending the project to provide real-time sunspot predictions using continuously updated data.
- **Model Tuning:** In-depth hyperparameter tuning for Prophet models to enhance forecast accuracy and precision.
