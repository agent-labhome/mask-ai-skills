# E-commerce Price Monitoring Skill

## Description
Track competitor prices, automatically adjust your pricing, and maximize profits with intelligent price monitoring and repricing strategies.

## Use Cases
- Competitor price tracking
- Dynamic pricing automation
- MAP violation detection
- Price alert systems
- Margin optimization

## Instructions

### Setting Up Price Monitoring

**1. Choose Monitoring Method:**

| Method | Cost | Features |
|--------|------|----------|
| Manual monitoring | Free | Time-consuming |
| Price tracking tools | $20-500/mo | Automated, comprehensive |
| Custom API integration | $100+/mo | Fully customized |

**2. Popular Tools:**

| Tool | Best For | Price |
|------|----------|-------|
| Prisync | E-commerce | $99/mo |
| Price2Spy | Enterprise | $199/mo |
| Competera | Retail | Custom |
| Feedvisor | Amazon | Custom |

### Building Custom Price Monitor

**Basic Python Script:**
```python
import requests
from bs4 import BeautifulSoup
import time

def get_price(url):
    headers = {'User-Agent': 'Mozilla/5.0'}
    response = requests.get(url, headers=headers)
    soup = BeautifulSoup(response.text, 'html.parser')
    # Adjust selector based on site
    price = soup.select_one('.price').text
    return float(price.replace('$', ''))

def check_prices():
    competitors = {
        'Amazon': 'https://amazon.com/product',
        'Walmart': 'https://walmart.com/product'
    }
    
    my_price = 29.99
    
    for name, url in competitors.items():
        comp_price = get_price(url)
        diff = my_price - comp_price
        
        if diff > 5:
            send_alert(f"Price gap: {name} is ${comp_price}")
        elif diff < -10:
            adjust_my_price(comp_price)
```

### Dynamic Pricing Strategies

**1. Cost-Plus Pricing:**
```
Price = (Cost + (Cost × Margin%))
```

**2. Competitive Pricing:**
```
Price = Market Average × (1 ± Adjustment%)
```

**3. Value-Based Pricing:**
```
Price = Customer Perceived Value - Discount
```

**4. Algorithmic Pricing:**
```
New Price = Current Price × (1 + (Demand Index × Factor))
```

### Repricing Rules

**For Amazon:**
- Keep within Buy Box range
- Respect MAP (Minimum Advertised Price)
- Factor in FBA fees
- Consider velocity (fast-moving = higher price)

**For Shopify:**
- Match competitors or beat by X%
- Factor shipping costs
- Consider customer lifetime value

### Alert Systems

**Setup Notifications:**
```python
import smtplib

def send_alert(subject, message):
    # Use SendGrid, AWS SES, or similar
    server = smtplib.SMTP('smtp.gmail.com', 587)
    server.sendmail(from_addr, to_addr, msg)
```

**Slack Integration:**
```python
def slack_notify(text):
    webhook_url = 'https://hooks.slack.com/...'
    requests.post(webhook_url, json={'text': text})
```

### Best Practices

1. **Monitor 5-10 key competitors**
2. **Update prices 1-2x daily max**
3. **Set floor/ceiling prices**
4. **Factor in all costs** (shipping, fees, etc.)
5. **Track historical data**
6. **Test different strategies**

## ROI Calculation

```
Price Monitoring Investment:
- Tool cost: $100/mo
- Time spent: 5 hrs/mo ($50 value)

Savings/Revenue:
- Competitor undercutting prevented: $500/mo
- Optimal pricing gains: $300/mo
- MAP violations caught: $200/mo

Net Benefit: $950/mo - $150/mo = $800/mo profit
