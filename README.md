**Furniture Sales Forecasting**
This project focuses on forecasting furniture sales using time series analysis techniques. We apply the ARIMA model to predict future sales based on historical transactional data, allowing better decision-making in inventory and supply chain planning.

Project Objective:
To forecast furniture product sales for the upcoming year by analyzing historical data using statistical modeling techniques. The goal is to build a predictive model that can assist in optimizing business operations and planning.

Dataset Description
- The dataset contains sales transactions filtered to include only Furniture category.
- Key fields:
  - Order Date
  - Sales
  - (Other fields may exist but are not used for time series)

Techniques Used:
- Data filtering and cleaning
- Time-based grouping and sorting
- Resampling to ensure equally spaced dates
- Manual Train-Test Split
- ARIMA (AutoRegressive Integrated Moving Average) model
- Export of forecast results to Excel

Model Used
ARIMA (AutoRegressive Integrated Moving Average)
   - Used to capture temporal structures in sales data.
   - Parameters `(p, d, q)` are tuned manually.
   - Model trained on historical sales data for forecasting 1-year ahead.

Output:
- The forecasted sales are exported to:  
  `TimeSeriesOutput_ARIMA.xlsx`

Results:
- The model provides a 1-year forward forecast of sales based on historical trends.
- Results can be used to support business planning and inventory management.

Future Improvements
- Incorporate **seasonality** using SARIMA
- Add **external regressors** (e.g., marketing events, holidays) using SARIMAX
- Visualize actual vs forecasted values
- Add evaluation metrics like RMSE, MAPE

Requirements:
- Python 3.x
- pandas
- numpy
- matplotlib
- statsmodels
- openpyxl (for Excel output)

Install dependencies via:
bash
pip install pandas numpy matplotlib statsmodels openpyxl
