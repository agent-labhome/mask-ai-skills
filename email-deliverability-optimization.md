---
name: email-deliverability-optimization
description: 邮件投递优化 - Gmail/Outlook投递率、垃圾邮件处理、域名配置。适用于：(1) 邮件进箱率优化 (2) SPF/DKIM/DMARC配置 (3) 域名信誉修复 (4) 邮件营销 (5) 企业邮箱
---

# 邮件投递优化

## 核心概念

- **投递率** - 到达收件箱 vs 垃圾邮件
- **打开率** - 实际阅读
- **信誉** - 发件域名/IP评分

## 关键配置

### SPF (Sender Policy Framework)
```
v=spf1 include:_spf.google.com ~all
```

### DKIM (DomainKeys Identified Mail)
- 公钥/私钥加密签名
- 需在DNS添加记录

### DMARC (Domain-based Message Authentication)
- 策略：none/quarantine/reject
- 报告：aggregate/forensic

## Gmail优化

- 避免敏感词（free, guarantee, $$$）
- 图片/文本比例1:1
- 退订按钮必需
- 发送频率稳定
- 互动好的用户优先

## 信誉修复

1. 停止发送（1-2周）
2. 清理列表（退信/不活跃）
3. 预热新域名
4. 内容优化
5. 监控投诉率

## 工具推荐

| 工具 | 用途 |
|------|------|
| Mailgun/SendGrid | 专业发送 |
| Google Postmaster | 信誉监控 |
| MXToolbox | 配置检查 |
| Litmus | 预览测试 |
