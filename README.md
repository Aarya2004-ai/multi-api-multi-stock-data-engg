
# Multi-API Stock Market Data Pipeline with Sentiment Analysis

## Overview

This project demonstrates a scalable data engineering pipeline that ingests stock market data from multiple APIs (Alpha Vantage, Finnhub, and Financial Modeling Prep) into Azure Data Lake Storage (ADLS). The pipeline is designed with dynamic parameters in Azure Data Factory (ADF) to handle multiple stocks and APIs without manual reconfiguration.

Additionally, the project includes a sentiment analysis layer that enriches financial data with market sentiment for enhanced insights.

## Key Features

* Multi-API Integration – Collects historical and daily stock data from three APIs.
* Dynamic Pipelines – Uses parameterized ADF pipelines with Lookup + ForEach activities to dynamically fetch data for different stocks and APIs.
* Scalable Storage – Organized raw data in a layered approach for historical and daily ingestion, ensuring easy extension to new stocks/APIs.
* Parquet Transformation – Data stored in Parquet format for optimized querying and downstream analytics.
* Sentiment Analysis – Performs NLP-based sentiment scoring on stock-related news to provide contextual market insights.

## Tech Stack

* Azure Data Factory – Orchestration & dynamic pipelines
* Azure Data Lake Storage – Raw & curated data layers
* APIs – Alpha Vantage, Finnhub, FMP
* Python – Sentiment analysis
* Parquet – Optimized storage format

## Future Enhancements

* Add more tickers dynamically via config files (JSON/CSV).
* Automate downstream reporting with Power BI dashboards.
* Extend NLP sentiment model for multi-language news.

---

Do you want me to make this **GitHub README** more **visual** (like including a flow diagram of your pipeline instead of the folder structure) so it looks portfolio-polished?
