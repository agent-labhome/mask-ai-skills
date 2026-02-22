# Auto Agent System

帮助你搭建自动运行的AI Agent系统。

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## 核心能力

### 1. 系统架构
- Supabase数据库
- Next.js前端
- VPS服务器

### 2. 核心表
- proposals (提案)
- missions (任务)
- steps (步骤)
- events (事件)

### 3. Heartbeat
- 每5分钟触发
- 评估触发器
- 处理队列
- 恢复任务

### 4. Agent设计
- 角色设定
- 工具定义
- 记忆系统
- 关系动态

## 架构示例

```
VPS: Agent执行
  ↓
Vercel: 任务调度
  ↓
Supabase: 数据存储
```

### 核心流程

```
Proposal → Mission → Step → Event → Proposal
(闭环循环)
```

### Cap Gates

```javascript
const STEP_KIND_GATES = {
  write_content: checkWriteContentGate,
  post_tweet: checkPostTweetGate,
};

async function checkPostTweetGate(sb) {
  const quota = await getPolicy(sb, 'x_daily_quota');
  const todayCount = await countTodayPosted(sb);
  
  if (todayCount >= quota.limit) {
    return { ok: false, reason: 'Quota full' };
  }
  return { ok: true };
}
```

### Policy Table

```sql
CREATE TABLE ops_policy (
  key TEXT PRIMARY KEY,
  value JSONB NOT NULL DEFAULT '{}'
);
```

---

## 成本

- VPS: $8/月
- Supabase: 免费
- Vercel: 免费
- LLM: $20-50/月

**总计: $28-58/月**

---

## 变现方式

- 开发: $2000-10000
- 咨询: $500-2000
- 培训: $299-999

---

*Price: $49*
*Category: Technology*
*Tags: ai-agent, automation, supabase, nextjs, autonomous*


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /auto-agent-system
- Auto Agent System
