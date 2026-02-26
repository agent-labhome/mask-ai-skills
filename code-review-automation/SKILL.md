# Code Review Automation

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Description
AI-powered code review automation - automatically analyze, critique, and suggest improvements for code submissions.

## Use Cases
- Automated pull request reviews
- Code quality scoring
- Security vulnerability detection
- Best practices enforcement
- Performance optimization suggestions

## Instructions

### Setting Up Code Review Bot

1. **Choose Platform:**
   - GitHub: Use GitHub Actions + CodeQL
   - GitLab: Use GitLab CI/CD
   - Custom: Use webhooks + LLM API

2. **Basic Workflow:**
   ```
   1. Developer submits PR
   2. Webhook triggers review pipeline
   3. LLM analyzes code changes
   4. Review comments posted automatically
   ```

### Prompts for Code Review

**Security Review:**
```
Review this code for security vulnerabilities:
- SQL injection
- XSS attacks
- Authentication issues
- Data exposure
Provide specific fix suggestions.
```

**Performance Review:**
```
Analyze for performance issues:
- N+1 queries
- Unnecessary loops
- Missing indexes
- Memory leaks
Suggest optimizations with code examples.
```

**Code Quality:**
```
Rate this code on:
- Readability (1-10)
- Maintainability (1-10)
- Testability (1-10)
- Documentation quality
Provide specific improvement suggestions.
```

### Tools & Integrations

**GitHub Actions Example:**
```yaml
name: AI Code Review
on: [pull_request]
jobs:
  review:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Run AI Review
        env:
          OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
        run: |
          # Extract diff and send to LLM
```

**Recommended Tools:**
- CodeQL (security scanning)
- SonarQube (quality gates)
- DeepCode (AI review)
- GPT Review (LLM-based)

### Best Practices

1. **Don't replace human review** - AI assists, humans decide
2. **Set clear guidelines** - Define what's acceptable
3. **Handle false positives** - Allow developers to override
4. **Track patterns** - Learn from recurring issues
5. **Integrate early** - Review before merge

## Pricing Tiers

- Free: Basic syntax checks
- $10/mo: AI-powered review (500 reviews)
- $50/mo: Enterprise (unlimited + custom rules)


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /code-review-automation
- Code Review Automation
