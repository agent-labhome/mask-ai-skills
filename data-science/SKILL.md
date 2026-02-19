# Data Science with Python

帮助你用Python做数据分析。

## 核心能力

### 1. 数据处理
- Pandas
- NumPy
- 数据清洗
- 特征工程

### 2. 数据可视化
- Matplotlib
- Seaborn
- Plotly
- Streamlit

### 3. 机器学习
- Scikit-learn
- XGBoost
- 特征选择
- 模型评估

### 4. 实战项目
- 销售预测
- 用户分析
- 推荐系统
- NLP

## 使用示例

```
用户: 想学数据分析

助手:
## 📊 Python数据科学

### Pandas基础

```python
import pandas as pd

# 读取数据
df = pd.read_csv("data.csv")

# 查看数据
print(df.head())
print(df.info())

# 数据清洗
df = df.dropna()
df = df[df["age"] > 0]

# 分组统计
df.groupby("category").sum()
```

### 数据可视化

```python
import matplotlib.pyplot as plt

plt.figure(figsize=(10, 6))
plt.plot(x, y)
plt.title("Sales Trend")
plt.show()
```

### 机器学习

```python
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier

X_train, X_test, y_train, y_test = train_test_split(X, y)
model = RandomForestClassifier()
model.fit(X_train, y_train)
score = model.score(X_test, y_test)
```

### Streamlit仪表盘

```python
import streamlit as st

st.title("My Dashboard")
st.line_chart(data)
```
```

---

## 工具

- Jupyter
- Pandas
- Scikit-learn
- Streamlit

---

## 变现方式

- 分析: $100-1000
- 咨询: $100-500
- 培训: $99-499

---

*Price: $29*
*Category: Data*
*Tags: data-science, python, pandas, machine-learning, analytics*
