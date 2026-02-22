# Line Bot

帮助你开发LINE机器人，从功能到部署。

## 核心能力

### 1. 基础功能
- 自动回复
- 消息处理
- 按钮模板
- Flex Message

### 2. 进阶功能
- 群管理
- 投票问卷
- 文件处理
- 支付集成

### 3. 实用案例
- 客服机器人
- 预约系统
- 数据收集
- 定时任务

### 4. 部署运维
- Heroku部署
- Vercel/Render
- 监控告警
- 扩展优化

## 使用示例

```
用户: 我想做一个天气查询机器人

助手:
## 🌤️ LINE天气机器人

### 技术栈
- Node.js + @lineSDK
- 天气API: OpenWeatherMap
- 部署: Vercel/Render

### 核心代码
```javascript
const line = require('@line/sdk');
const client = new line.Client('CHANNEL_ACCESS_TOKEN');

app.post('/webhook', line.middleware('CHANNEL_SECRET'), (req, res) => {
  Promise.all(req.body.events.map(handleEvent))
    .then(() => res.end())
    .catch(err => {
      console.error(err);
      res.status(500).send('Error');
    });
});

async function handleEvent(event) {
  if (event.type !== 'message' || event.message.type !== 'text') {
    return;
  }
  
  const city = event.message.text;
  const weather = await getWeather(city);
  
  return client.replyMessage(event.replyToken, {
    type: 'text',
    text: weather
  });
}
```

### 功能扩展
1. 添加每日天气提醒
2. 支持多个城市
3. 发送天气图片
4. 设置位置提醒
```

---

## 常用SDK

- @line/sdk (Node.js)
- line-bot-sdk-python (Python)
- line-sdk (Go)
- Firebase Functions

---

## 变现方式

- 定制开发: $100-1000
- SaaS服务: $20-200/月
- 模板销售: $29-99
- 日本/台湾市场定向

---

*Price: $39*
*Category: Development*
*Tags: line, bot, messaging, japan, taiwan, automation*


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /line-bot
- Line Bot
