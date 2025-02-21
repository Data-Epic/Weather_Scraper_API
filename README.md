# **Project: Weather scraper API**


## Goal:
Extract weather data from https://www.timeanddate.com/weather/nigeria/, select 3 state of choice.Build a FastAPI-based web service that scrapes data from a website, cleans it using regex (if needed), and writes the cleaned data to a Google Sheet. The service will expose a FastAPI endpoint that can be tested via the interactive /docs interface.


Project Structure

```
weather_api/
    ├── .gitignore
    ├── .env.example
    ├── README.md
    ├── main.py
    ├── pyproject.toml
    ├── poetry.lock
    ├── scraper/
    │   ├── __init__.py
    │   ├── scraper.py
    │   └── google_sheet.py
    └── tests/
        ├── __init__.py
        └── test_scraper.py

    
```

### **Features:**

    1. FastAPI Endpoint: A get endpoint that pulls current weather data. Runs the scraper, processes the data, and writes the results to Google Sheets.
    2. Dependency Management: Use poetry for package management.
    3. Virtual Environment: Use venv for isolated Python environments.
    4. Web Scraping: Extract specific information from a target webpage.
    5. Data Cleaning
    6. Write to Google Sheets: Use gspread to authenticate and update a Google Sheet.
    7. API Documentation: Interactive Swagger UI (/docs) to test the API.