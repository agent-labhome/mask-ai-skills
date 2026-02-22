# Selenium Automation

帮助你用Selenium实现浏览器自动化。

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## 核心能力

### 1. 基础
- 安装
- WebDriver
- 定位元素
- 基本操作

### 2. 操作
- 点击输入
- 等待
- 滚动
- 截图

### 3. 高级
- iframe
- 弹窗
- 下拉框
- 上传

### 4. 实战
- 测试自动化
- 数据抓取
- 表单填写
- 定时任务

## 使用示例

```
用户: 想自动化浏览器

助手:
## 🌐 Selenium指南

### 安装

```python
pip install selenium
pip install webdriver-manager
```

### 基础代码

```python
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.chrome.service import Service

driver = webdriver.Chrome()
driver.get("https://example.com")

# 找到元素
element = driver.find_element(By.ID, "username")
element.send_keys("myusername")

# 点击
button = driver.find_element(By.CLASS_NAME, "submit")
button.click()

driver.quit()
```

### 等待

```python
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC

wait = WebDriverWait(driver, 10)
element = wait.until(EC.presence_of_element_located((By.ID, "result")))
```

### 定位

- By.ID
- By.NAME
- By.CLASS_NAME
- By.XPATH
- By.CSS_SELECTOR
```

---

## 工具

- ChromeDriver
- GeckoDriver
- WebDriver Manager

---

## 变现方式

- 测试开发: $100-500
- 咨询: $100-500
- 培训: $99-499

---

*Price: $29*
*Category: Development*
*Tags: selenium, automation, testing, python, browser*


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /selenium-automation
- Selenium Automation
