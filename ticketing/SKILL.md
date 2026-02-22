## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Purpose
This skill enables the creation of structured, actionable briefs for ticketing systems (Jira, GitHub Issues, Linear, etc.) from natural language descriptions.

## Input Format
Users provide:
- A description of the issue/feature
- Optional context about priority, environment, or requirements
- May include phrases like \"create a ticket for...\" or \"brief for...\"

## Output Format
A structured brief with these sections:

### 1. Title
- Clear, concise summary (under 60 chars)
- Starts with action verb when applicable
- Includes system/component when relevant

### 2. Description
- Problem statement or goal
- Current state vs desired state
- User impact/value

### 3. Acceptance Criteria

## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /ticketing
- Ticketing
