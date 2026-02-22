-e {"id":"e96dd4f7-32cb-4e2d-b70a-5e51672bbd92","object":"chat.completion","created":1771650728,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Kanban - SKILL.md

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata

```yaml
name: Kanban
version: 1.0.0
author: Your Name/Organization
description: A Kanban board implementation for task and project management with drag-and-drop functionality
category: Productivity
tags: [project-management, tasks, workflow, productivity, agile]
license: MIT
repository: https://github.com/yourusername/kanban-skill
dependencies:
  - react
  - react-dnd
  - react-dnd-html5-backend
  - uuid
  - date-fns
prerequisites:
  - Node.js 16+
  - npm or yarn
  - Basic React knowledge
compatibility:
  web: true
  mobile: responsive
  desktop: true
```

## Overview

Kanban is a visual task management system that helps teams and individuals organize work using columns and cards. This implementation provides a fully functional Kanban board with drag-and-drop capabilities, local storage persistence, and customizable workflows.

## Installation

### Prerequisites
- Node.js 16 or higher
- npm or yarn package manager
- React project setup

### Installation Steps

1. **Install dependencies:**
```bash
npm install react-dnd react-dnd-html5-backend uuid date-fns
# or
yarn add react-dnd react-dnd-html5-backend uuid date-fns
```

2. **Add Kanban component to your project:**
```bash
# Copy the Kanban component files to your project
mkdir -p src/components/Kanban
cp Kanban.jsx src/components/Kanban/
cp Kanban.css src/components/Kanban/
```

3. **Import and use in your application:**
```jsx
import { DndProvider } from 'react-dnd';
import { HTML5Backend } from 'react-dnd-html5-backend';
import Kanban from './components/Kanban/Kanban';

function App() {
  return (
    <DndProvider backend={HTML5Backend}>
      <Kanban />
    </DndProvider>
  );
}
```

## Configuration

### Initial Setup

The Kanban board comes with default columns and sample data. You can customize this by passing props:

```jsx
<Kanban 
  initialColumns={customColumns}
  boardTitle=\"My Project Board\"
  showStats={true}
 "},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":19,"completion_tokens":500,"total_tokens":519,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":19},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /kanban
- Kanban
