# Web Scraping – HTML Table Extraction

## Project Overview

A simple web scraping practice project using **Python and BeautifulSoup** to extract a table from a website.

## Tools Used

* Python
* BeautifulSoup
* Requests
* Google Colab

## What I Did

* Accessed a webpage using Python.
* Parsed the webpage HTML using BeautifulSoup.
* Located the required HTML table.
* Extracted the table headers.
* Extracted the table data from the webpage.
* Displayed the extracted table in a structured format.

## Code

```python
import requests
from bs4 import BeautifulSoup

response = requests.get(url)

soup = BeautifulSoup(response.text, 'html.parser')

table1 = soup.find('table')

headers2 = table1.find('tr')

cols1 = [th.get_text(strip=True) for th in headers2 if th.get_text(strip=True)]

cols1
```

## Outcome

Successfully extracted the required HTML table from the website using **BeautifulSoup** and brought the data into Python for further use.

## Key Learning

Learned the basic process of identifying and extracting data from an HTML table using BeautifulSoup.
