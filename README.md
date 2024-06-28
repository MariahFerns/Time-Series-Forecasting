# Time-series-forecasting

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
     ![image](https://github.com/MariahFerns/Time-series-forecasting/assets/165193476/a118335b-f413-418e-8e37-acf99e032505)
   - Used auto ARIMA (SARIMA) for time series forecasting.
     ![image](https://github.com/MariahFerns/Time-series-forecasting/assets/165193476/118e7a15-4774-4783-b8b0-0f10a0331179)
   - Applied Facebook's Prophet for another time series forecasting approach.
     ![image](https://github.com/MariahFerns/Time-series-forecasting/assets/165193476/9c3e760e-1849-478f-a6a8-9bdc9ca44d74)
   - Developed a deep learning model using LSTM for more complex patterns.
     ![image](https://github.com/MariahFerns/Time-series-forecasting/assets/165193476/a81b8f8a-f309-4d79-ab06-d824b34c403d)

## Results
- **EDA Findings**:
  - Identified peak sales periods and trends over different time frames.
    ![image](https://github.com/MariahFerns/Time-series-forecasting/assets/165193476/f6584a49-9c6e-444d-8be3-69e4040145df)
  - Highlighted the most popular items and top-performing stores.

- **Model Performance**:
  - Linear Regression, Random Forest, and XGBoost were evaluated using RMSE. Random Forest performed consistently well across all stores.
    ![image](https://github.com/MariahFerns/Time-series-forecasting/assets/165193476/93d6c160-f616-4edd-b282-425ea918b406)
  - SARIMA and Prophet models provided insights into seasonality and trends.
    ![image](https://github.com/MariahFerns/Time-series-forecasting/assets/165193476/800145e8-a3c9-4caf-a565-c9fbbe4fb1ff)
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
