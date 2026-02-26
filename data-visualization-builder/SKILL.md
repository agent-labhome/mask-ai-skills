# Data Visualization Builder

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Description
Create compelling data visualizations and dashboards - from basic charts to interactive dashboards that tell stories with your data.

## Use Cases
- Business dashboards
- Analytics reports
- Data storytelling
- Real-time monitoring
- Presentation visuals

## Instructions

### Visualization Tools Stack

**No-Code/Low-Code:**
| Tool | Best For | Price |
|------|----------|-------|
| Tableau | Enterprise analytics | $70/user/mo |
| Power BI | Microsoft ecosystem | $10/mo |
| Looker | Embedded analytics | $100+/mo |
| Google Data Studio | Simple dashboards | Free |
| Obsidian + Dataview | Personal knowledge | Free |

**Code-Based:**
| Tool | Use Case |
|------|----------|
| D3.js | Custom visualizations |
| Chart.js | Simple web charts |
| Python (Matplotlib/Seaborn) | Data analysis |
| R (ggplot2) | Statistical graphics |

### Choosing the Right Chart

| Data Type | Best Chart |
|-----------|------------|
| Trends over time | Line chart |
| Part-to-whole | Pie/Donut |
| Comparison | Bar chart |
| Distribution | Histogram |
| Correlation | Scatter plot |
| Ranking | Horizontal bar |
| Single number | KPI card |

### Building Dashboards

**1. Define KPIs First:**
```
Dashboard Goals:
- Sales performance
- User growth
- Revenue metrics
- Customer health
```

**2. Layout Principles:**
```
+----------------------------------+
|  KPI Cards (4 across)           |
+----------------------------------+
|  Main Chart    |  Secondary      |
|  (2/3 width)   |  Chart (1/3)    |
+----------------------------------+
|  Detail Table                      |
+----------------------------------+
```

**3. Color Strategy:**
- Primary brand color: KPIs
- Secondary: Comparisons
- Alert colors: Warnings (red/yellow)
- Background: Light/neutral

### Code Examples

**Python (Matplotlib):**
```python
import matplotlib.pyplot as plt
import pandas as pd

# Sales trend
plt.figure(figsize=(12, 6))
plt.plot(df['date'], df['sales'], marker='o')
plt.title('Monthly Sales Trend')
plt.xlabel('Month')
plt.ylabel('Revenue ($)')
plt.grid(True)
plt.savefig('sales_trend.png')
```

**JavaScript (Chart.js):**
```javascript
new Chart(ctx, {
  type: 'line',
  data: {
    labels: ['Jan', 'Feb', 'Mar'],
    datasets: [{
      label: 'Revenue',
      data: [10000, 15000, 12000],
      borderColor: '#4F46E5'
    }]
  },
  options: {
    responsive: true,
    plugins: {
      legend: { position: 'top' }
    }
  }
});
```

**Google Data Studio Formula:**
```
CASE
  WHEN Score < 50 THEN "Needs Attention"
  WHEN Score < 80 THEN "On Track"
  ELSE "Exceeding"
END
```

### Interactive Dashboards

**Real-Time Updates:**
```javascript
// Fetch data every 30 seconds
setInterval(async () => {
  const data = await fetch('/api/metrics');
  updateChart(data);
}, 30000);
```

**Filtering:**
- Date range pickers
- Dropdown filters (category, region)
- Multi-select for comparison

### Best Practices

1. **Start with why** - What's the decision this supports?
2. **Simplify** - Less is more
3. **Use annotations** - Explain anomalies
4. **Mobile-first** - Consider smaller screens
5. **Test with users** - Validate insights

### Data Storytelling

**Structure:**
1. **Headline** - Key insight (e.g., "Sales up 20%")
2. **Supporting chart** - Visual evidence
3. **Context** - Why it matters
4. **Call to action** - What to do next

**Prompt for AI Help:**
```
Create a data story from this dataset:
[DATA]

Format:
- Main insight
- Supporting evidence
- Business implication
- Recommended action
```

## Tools Comparison

| Tool | Learning Curve | Customization | Cost |
|------|----------------|---------------|------|
| Tableau | Medium | High | $$$ |
| Power BI | Easy | Medium | $ |
| Data Studio | Easy | Low | Free |
| D3.js | Hard | Very High | Free |
| Python | Medium | High | Free |


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /data-visualization-builder
- Data Visualization Builder
