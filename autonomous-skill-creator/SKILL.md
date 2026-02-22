# Autonomous Skill Creator

帮助你每小时自动创建AI Skills。

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## 核心能力

### 1. 读取共识记忆
- 从 consensus.md 获取当前任务
- 理解目标和上下文

### 2. 创建新Skill
- 分析市场需求
- 创建 SKILL.md
- 保存到 skills/ 目录

### 3. 更新共识
- 记录完成的任务
- 设置下一步行动

### 4. Git同步
- 自动commit
- 自动push

## 执行流程

```
1. 读取 memories/consensus.md
2. 解析 "Next Action"
3. 创建对应Skill
4. 更新 consensus.md
5. Git commit + push
```

## 使用示例

```
用户: 创建一个Twitter Growth技能

助手:
## 🐦 Twitter Growth Skill

# Twitter Growth Expert

帮助你增长Twitter粉丝。

## 核心能力

### 1. 内容策略
- 推文类型
- 发布频率
- 互动技巧

### 2. 增长技巧
- 标签使用
- 时间优化
- 社区参与

### 3. 工具
- 管理工具
- 分析工具
- 自动化

## 使用示例

...

---
*Price: $19*
*Category: Marketing*
*Tags: twitter, growth, social-media*
```

更新共识记忆！


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /autonomous-skill-creator
- Autonomous Skill Creator
