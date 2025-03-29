# Mars Web Scraping & Weather Data Analysis

## Overview

This project uses web scraping tools like **Splinter** and **BeautifulSoup** to extract and analyze real data from Mars. It includes:

- Scraping recent Mars news headlines and preview text.
- Scraping a table of Mars weather data and performing statistical analysis and visualizations.

The goal is to demonstrate skills in web scraping, data cleaning, transformation, and exploratory data analysis.

---

## Part 1: Mars News

Automated browsing was used to visit a Mars News website. Using BeautifulSoup, we extracted the latest article headlines and corresponding preview text. Each article was stored in a dictionary with `title` and `preview` keys, and the full collection was stored in a list of dictionaries.

Example format:

```python
{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously..."}
```

This structured data could be saved or used for further natural language analysis.

---

## Part 2: Mars Weather Data Analysis

Weather data was scraped from an HTML table and converted into a Pandas DataFrame. All values were cleaned and converted to appropriate types (`int`, `float`, `datetime`) for analysis.

### 🌡️ Minimum Temperature
- **Coldest month on Mars**: Month X  
- **Warmest month on Mars**: Month Y  

Monthly averages show that Mars experiences a noticeable seasonal temperature pattern.

### 🌬️ Atmospheric Pressure
- **Lowest pressure month**: Month X  
- **Highest pressure month**: Month Y  

Atmospheric pressure also changes with the Martian seasons, likely due to polar ice cap activity and dust storms.

### 🪐 Martian Year Length
By plotting minimum daily temperatures over Earth dates:

- One full Martian year appears to span approximately **680 Earth days**, matching the known value of about **687 Earth days**.

---

## Output

The cleaned and structured weather dataset was exported as a CSV file:  
`mars_weather_data.csv`

---

## Tools Used

- Python  
- Pandas  
- BeautifulSoup  
- Splinter  
- Matplotlib
