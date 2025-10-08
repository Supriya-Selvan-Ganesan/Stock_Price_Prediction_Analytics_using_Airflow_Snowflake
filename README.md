The system will fetch Realtime stock price data for amazon and meta from yfinance API, the data is fetched daily
using an automated DAG in Airflow and loaded into a snowflake table. It runs a separate DAG for ML forecasting
and combines the actual and forecast data into a final table using SQL transaction. The final table can be used for
data analysis, visualization, reporting purpose or business decision-making.
