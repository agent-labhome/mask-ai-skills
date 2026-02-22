# Customer Segmentation

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata
- **Domain**: Marketing, Business Intelligence, Customer Relationship Management (CRM)
- **Complexity**: Intermediate
- **Key Techniques**: Clustering (K-Means, DBSCAN, Hierarchical), RFM Analysis, Dimensionality Reduction (PCA), Data Visualization
- **Tools**: Python (scikit-learn, pandas, matplotlib), SQL, Excel/Google Sheets
- **Related Skills**: Data Analysis, Statistics, Business Acumen, Data Visualization

## What is Customer Segmentation?

Customer segmentation is the practice of dividing a customer base into groups of individuals that are similar in specific ways relevant to marketing, such as demographics, purchasing behavior, or engagement patterns. This enables businesses to target groups effectively, allocate marketing resources efficiently, and develop tailored strategies for different customer types.

## Core Concepts

### 1. **Segmentation Approaches**
- **Demographic**: Age, gender, income, education
- **Geographic**: Location, climate, urban/rural
- **Psychographic**: Lifestyle, values, personality
- **Behavioral**: Purchase history, usage rate, brand loyalty
- **RFM Analysis**: Recency, Frequency, Monetary value

### 2. **Common Segmentation Models**
- **RFM Segmentation**: Simple yet powerful method using three metrics
- **K-Means Clustering**: Unsupervised learning to find natural groupings
- **Hierarchical Clustering**: Creates a tree of clusters
- **DBSCAN**: Density-based clustering for irregular shapes
- **Cohort Analysis**: Grouping customers by acquisition date

## Practical Implementation

### Step 1: Data Collection & Preparation
```python
import pandas as pd
import numpy as np

# Load customer data
df = pd.read_csv('customer_data.csv')

# Calculate RFM metrics
snapshot_date = df['InvoiceDate'].max() + pd.Timedelta(days=1)
rfm = df.groupby('CustomerID').agg({
    'InvoiceDate': lambda x: (snapshot_date - x.max()).days,  # Recency
    'InvoiceNo': 'count',  # Frequency
    'TotalPrice': 'sum'  # Monetary
})."},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":18,"completion_tokens":450,"total_tokens":468,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":18},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /customer-segmentation
- Customer Segmentation
