# ⏰Time-series-forecasting

## Introduction
In today's competitive market, accurate sales forecasting is crucial for making informed business decisions. This project aims to predict the demand for various items across restaurants, helping companies optimize their inventory and staffing decisions. By leveraging machine learning and deep learning techniques, we strive to improve the accuracy of sales forecasts.

## Data Description
We utilized three primary datasets:

1. **restaurants.csv**:
   - `id`: Unique identification of the restaurant.
   - `name`: Name of the restaurant.

2. **items.csv**:
   - `id`: Unique identification of the item.
   - `store_id`: Unique identification of the store.
   - `name`: Name of the item.
   - `kcal`: Caloric content of the item.
   - `cost`: Unit price of the item.

3. **sales.csv**:
   - `date`: Date of purchase.
   - `item`: Name of the item bought.
   - `price`: Unit price of the item.
   - `item_count`: Total count of the items bought on that day.

## Methodology
The project was divided into several key tasks:

1. **Data Wrangling**:
   - Imported and cleaned the datasets.
   - Merged datasets to create a comprehensive data frame.

2. **Exploratory Data Analysis (EDA)**:
   - Analyzed sales patterns over time.
   - Investigated sales variations across different days, months, and quarters.
   - Compared the performance of different restaurants and identified popular items.

3. **Forecasting**:
   - Implemented machine learning models: Linear Regression, Random Forest Regressor, and XGBoost.
   - Used auto ARIMA (SARIMA) for time series forecasting.
   - Applied Facebook's Prophet for another time series forecasting approach.
   - Developed a deep learning model using LSTM for more complex patterns.

## Results
- **EDA Findings**:
  - Identified peak sales periods and trends over different time frames.
  - Highlighted the most popular items and top-performing stores.

- **Model Performance**:
  - Linear Regression, Random Forest, and XGBoost were evaluated using RMSE. Random Forest performed consistently well across all stores.
  - SARIMA and Prophet models provided insights into seasonality and trends.
  - LSTM model captured complex patterns and performed well on test data.

## Conclusion
This project provided valuable insights into sales patterns and forecasting accuracy. The models developed can help companies make data-driven decisions, improving their operational efficiency. Future work could explore more advanced models and additional data sources to enhance predictions further.

## Tools and Libraries
- **Programming Language**: Python
- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn, feature_engine, statsmodels, pmdarima, fbprophet, TensorFlow, Keras

## Folder Structure
- `data/`: Raw data files.
- `notebooks/`: Jupyter notebooks for each task.
- `src/`: Python scripts for data processing and modeling.
- `models/`: Saved trained models.
- `api/`: Api code (FastAPI).
- `docs/`: Documentation includeing Output files with plots and evaluation metrics.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/MariahFerns/Time-series-forecasting.git
   cd Time-series-forecasting

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt

3. Run the Jupyter notebook in the notebooks/ folder to reproduce the analysis and models.

