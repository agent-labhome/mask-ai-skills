# Browser Extensions Developer

帮助你开发浏览器插件。

## 核心能力

### 1. 基础概念
- Manifest V3
- 权限
- 后台脚本
- 内容脚本

### 2. 开发工具
- Chrome扩展
- Firefox附加
- VS Code
- 调试

### 3. 常见功能
- 弹出窗口
- 内容修改
- 快捷键
- 存储

### 4. 发布变现
- Chrome Web Store
- Firefox Add-ons
- 付费插件
- 捐赠

## 使用示例

```
用户: 想做浏览器插件

助手:
## 🔌 浏览器插件指南

### Manifest V3

```json
{
  "manifest_version": 3,
  "name": "My Extension",
  "version": "1.0",
  "permissions": ["storage"],
  "action": {
    "default_popup": "popup.html"
  },
  "background": {
    "service_worker": "background.js"
  }
}
```

### 内容脚本

```javascript
// content.js
console.log("Extension loaded!");

// 修改页面
document.body.style.background = "pink";

// 监听消息
chrome.runtime.onMessage.addListener((msg) => {
  console.log(msg);
});
```

### Popup

```html
<!-- popup.html -->
<!DOCTYPE html>
<html>
<body>
  <h1>Hello!</h1>
  <button id="btn">Click me</button>
  <script src="popup.js"></script>
</body>
</html>
```

### 发布

1. 打包: zip文件
2. Chrome: 开发者后台上传
3. Firefox: AMO上传
4. 收费: 付费扩展
```

---

## 工具

- Chrome扩展管理
- Extension Reloader
- Chrome DevTools

---

## 变现方式

- 付费: $5-50
- 捐赠
- 企业定制: $1000+

---

*Price: $29*
*Category: Development*
*Tags: browser-extension, chrome, firefox, plugins, javascript*
