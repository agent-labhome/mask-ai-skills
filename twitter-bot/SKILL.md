# Twitter Bot Developer

帮助你开发Twitter机器人。

## 核心能力

### 1. API使用
- Twitter API v2
- 认证方式
- 限流规则
- 免费vs付费

### 2. 功能开发
- 自动发推
- 自动回复
- 定时任务
- 数据分析

### 3. 工具
- Tweepy
- Twitter API
- Zapier
- 自建

### 4. 变现
- 自动化服务
- 账号管理
- 数据服务

## 使用示例

```
用户: 想做Twitter机器人

助手:
## 🐦 Twitter机器人指南

### API选择

**免费 (Basic):**
- $100/月
- 只能读
- 1个应用

**付费 (Pro):**
- $5000/月
- 读写都有
- 高级分析

### Tweepy示例

```python
import tweepy

auth = tweepy.OAuthHandler(API_KEY, API_SECRET)
auth.set_access_token(ACCESS_TOKEN, ACCESS_SECRET)

api = tweepy.API(auth)

# 发推
api.update_status("Hello from bot!")

# 搜索
tweets = api.search_tweets(q="AI")

# 自动回复
for tweet in mentions:
    api.update_status(
        f"@{tweet.user.screen_name} 谢谢！",
        in_reply_to_status_id=tweet.id
    )
```

### Zapier方案

- Trigger: RSS/New tweet
- Action: Post tweet / Send Slack
```

---

## 工具

- Tweepy (Python)
- Twitter API v2
- Zapier
- Typefully

---

## 变现方式

- 开发: $200-2000
- 咨询: $100-500
- 培训: $99-499

---

*Price: $29*
*Category: Development*
*Tags: twitter, bot, automation, python, api*
