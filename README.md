# **Bitcoin Today – Real-Time Price & Crypto News Dashboard**

Welcome to the **Bitcoin Today** project, a Streamlit application that brings together real-time Bitcoin price data and curated crypto news.  
This app integrates **API data ingestion**, **web scraping**, and **database storage**, providing a compact example of an end-to-end data engineering workflow.

---

## **Overview**

Bitcoin Today was built to explore how financial datasets and news sources can be combined into a single interactive dashboard.

The application retrieves:

- **Live Bitcoin price data** from the Alpha Vantage API  
- **Latest cryptocurrency articles** from the U.Today news site  
- **Persisted records** stored in Supabase  
- **Interactive visualisation** and analysis through Streamlit  

The project demonstrates how external APIs, web scraping, and storage layers can be combined to enrich financial insights.

---

## **Core Features**

### **Real-Time Bitcoin Price Retrieval**
Fetches the latest Bitcoin price using the **Alpha Vantage** API.  
The app uses structured JSON responses to extract daily price, open/close values, and time-series trends.

### **Crypto News Scraper**
Scrapes the U.Today website to retrieve:

- Latest crypto-related headlines  
- Article descriptions  
- Publication timestamps  
- Author names (when available)  

This allows the dashboard to display both market data and contextual news in one unified UI.

### **Streamlit Dashboard**
Interactive web interface built with Streamlit, offering:

- Bitcoin price panel  
- Latest news feed  
- Refresh and update logic  
- Error handling when APIs are unavailable  

Designed with a clear layout focused on usability.

### **Supabase Database Integration**
Supabase is used to store:

- Historical Bitcoin prices  
- Retrieved article metadata  
- Logging information  

The connection is handled through Streamlit’s secret configuration and PostgreSQL drivers.

---

## **Tech Stack**

- **Python** — API calls, web scraping, transformations  
- **Alpha Vantage API** — Bitcoin price data  
- **U.Today scraper** — news extraction  
- **Streamlit** — web UI  
- **Supabase** — database backend  
- **Requests / BeautifulSoup** — scraping and HTTP handling  
- **Pandas** — data manipulation  

---

## **Project Structure**

```
Project6_Bitcoin/
├── streamlit/                  # Streamlit application files
├── data/                       # Cached/processed data (if used)
├── utils/                      # Helper functions (API requests, scraping)
├── notebooks/                  # Optional analysis notebooks
└── README.md
```

---

## **Future Improvements**

- Add sentiment analysis to scraped news articles  
- Automate scheduled ingestion with a cloud function  
- Enhance time-series forecasting using Prophet or ARIMA  
- Add multi-cryptocurrency support (ETH, SOL, etc.)  
- Deploy to Streamlit Cloud with production API keys  

---

## **Author**

**Bruno Aro**  
Portfolio: https://bruno-aro.github.io  
