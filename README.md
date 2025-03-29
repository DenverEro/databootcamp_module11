# Mars Web Scraping & Weather Data Analysis

## Overview

This project uses web scraping tools like **Splinter** and **BeautifulSoup** to extract and analyze real data from Mars. It includes:

- Scraping recent Mars news headlines and preview text.
- Scraping a table of Mars weather data and performing data analysis on it.

The goal is to demonstrate skills in web scraping, data cleaning, and data visualization.

---

## Part 1: Mars News

Automated browsing was used to visit a Mars News website. Using BeautifulSoup, we extracted the latest headlines and preview snippets of news articles. The data was structured as a list of dictionaries and printed to verify successful scraping.

Example format:

```python
{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously..."}

---

## Part 2: Mars Weather Data Analysis

Weather data was scraped from an HTML table and converted into a pandas DataFrame. Data types were cleaned and converted for analysis.

### 🌡️ Minimum Temperature
- **Coldest month on Mars**: Month X  
- **Warmest month on Mars**: Month Y  

Mars exhibits a clear seasonal pattern in minimum daily temperatures.

### 🌬️ Atmospheric Pressure
- **Lowest pressure month**: Month X  
- **Highest pressure month**: Month Y  

Pressure varies seasonally, likely influenced by polar CO₂ cycles and dust storms.

### 🪐 Martian Year Length
By plotting minimum temperatures over time:

- A full Martian year appears to span about **680 Earth days**.
- This closely matches the known Martian year length of **687 Earth days**.

---

## Output

The weather dataset was exported as a CSV: `mars_weather_data.csv`

---

## Tools Used

- Python  
- Pandas  
- BeautifulSoup  
- Splinter  
- Matplotlib