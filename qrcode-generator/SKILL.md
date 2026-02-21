# SKILL.md - QR Code Generator

## Skill Name
qrcode-generator

## Description
生成各种类型的二维码 - URL、文本、WIFI、联系信息、支付码等。支持自定义颜色、logo嵌入、样式定制。

## Use Cases
- 创建可扫描的URL二维码
- 生成WIFI登录二维码
- 创建联系信息二维码(vCard)
- 支付二维码(微信/支付宝)
- 加密内容二维码

## Tools
- web_search: 搜索二维码生成工具和API
- web_fetch: 获取二维码生成服务文档

## Instructions

### 1. 确定二维码类型
- URL链接 → 使用URL二维码
- 纯文本 → 使用文本二维码
- WIFI信息 → 使用WIFI二维码(格式: WIFI:T:WPA;S:网络名;P:密码;;)
- 联系信息 → 使用vCard格式
- 支付 → 使用对应平台支付码

### 2. 生成方式
- 在线工具: qr-code-generator.com, qrcode.monster, create-qr-code.com
- API: goqr.me API, QRServer API
- Python库: qrcode, segno

### 3. 自定义选项
- 颜色: 前景色/背景色
- 大小: 像素尺寸
- 样式: 方块圆角、边距
- logo: 中间嵌入图片

## 示例Prompt
"生成一个指向 https://example.com 的二维码，蓝色前景色，白色背景"

## Related Skills
- link-shortener: 短链接生成
- barcode-generator: 条形码生成
