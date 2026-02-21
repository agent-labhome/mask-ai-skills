-e {"id":"ae823f9b-e9c6-4e23-a115-6bff8f87c9bb","object":"chat.completion","created":1771671590,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Web Scraping: A Practical Guide

## Metadata
- **Category**: Data Acquisition & Automation
- **Complexity**: Beginner to Advanced
- **Prerequisites**: Basic Python, HTML/CSS familiarity
- **Common Tools**: BeautifulSoup, Scrapy, Selenium, Requests
- **Related Skills**: Data Cleaning, API Integration, Data Analysis

## What is Web Scraping?

Web scraping is the automated extraction of data from websites. It involves programmatically accessing web pages, parsing HTML/XML content, and extracting structured information for analysis, storage, or integration with other systems.

## Core Concepts

### 1. **Legal and Ethical Considerations**
- **Check robots.txt**: `website.com/robots.txt`
- **Respect rate limits**: Add delays between requests
- **Review Terms of Service**: Some sites prohibit scraping
- **Identify yourself**: Use proper User-Agent headers
- **Don't overload servers**: Be a good internet citizen

### 2. **HTTP Fundamentals**
- GET/POST requests
- Status codes (200, 404, 403, 429)
- Headers (User-Agent, Cookies, Referer)
- Sessions and authentication

### 3. **HTML Structure**
- DOM (Document Object Model)
- CSS selectors and XPath
- HTML elements, attributes, and classes

## Practical Guide

### Level 1: Beginner (Static Pages)

**Tools**: `requests`, `BeautifulSoup`

```python
import requests
from bs4 import BeautifulSoup
import pandas as pd

# Basic scraping workflow
def scrape_basic(url):
    # 1. Fetch the page
    headers = {'User-Agent': 'Mozilla/5.0'}
    response = requests.get(url, headers=headers)
    
    # 2. Parse HTML
    soup = BeautifulSoup(response.content, 'html.parser')
    
    # 3. Extract data using CSS selectors
    titles = soup.select('.product-title')
    prices = soup.select('.price')
    
    # 4. Structure the data
    data = []
    for title, price in zip(titles, prices):
        data.append({
            'title': title.text.strip(),
            'price': price.text.strip()
        })
    
    return pd.DataFrame(data)

# Add polite scraping
import time
import random

def polite_scrape(urls):
    results = []
    for url in"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":21,"completion_tokens":500,"total_tokens":521,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":21},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
