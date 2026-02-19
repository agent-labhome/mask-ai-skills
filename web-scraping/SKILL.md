# Web Scraping Expert

帮助你抓取网页数据。

## 核心能力

### 1. 基础工具
- Requests
- BeautifulSoup
- Selenium
- Playwright

### 2. 反爬策略
- User-Agent
- 代理
- 请求频率
- 验证码

### 3. 数据存储
- CSV
- JSON
- 数据库
- API

### 4. 实战
- 电商数据
- 社交媒体
- 资讯网站
- 股票数据

## 使用示例

```
用户: 想抓取网站数据

助手:
## 🕷️ 网页抓取指南

### BeautifulSoup

```python
import requests
from bs4 import BeautifulSoup

url = "https://example.com"
response = requests.get(url)
soup = BeautifulSoup(response.text)

# 提取数据
titles = soup.find_all("h2")
for title in titles:
    print(title.text)
```

### Playwright (JS渲染)

```python
from playwright.sync_api import sync_playwright

with sync_playwright() as p:
    browser = p.chromium.launch()
    page = browser.new_page()
    page.goto("https://example.com")
    content = page.content()
    browser.close()
```

### 反爬策略

```python
headers = {
    "User-Agent": "Mozilla/5.0..."
}
response = requests.get(url, headers=headers)
```

### 数据存储

```python
import pandas as pd

df = pd.DataFrame(data)
df.to_csv("data.csv", index=False)
df.to_json("data.json", orient="records")
```
```

---

## 注意事项

1. 遵守robots.txt
2. 不要过度请求
3. 考虑法律风险

---

## 变现方式

- 数据服务: $100-1000
- 咨询: $100-500
- 培训: $99-499

---

*Price: $29*
*Category: Development*
*Tags: scraping, python, automation, data, requests*
