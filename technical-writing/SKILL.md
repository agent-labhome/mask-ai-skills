# SKILL.md: Technical Writing

## Metadata
- **Skill Domain:** Communication & Documentation
- **Proficiency Levels:** Beginner → Intermediate → Advanced → Expert
- **Related Skills:** Technical Communication, API Documentation, User Guides, Tutorials, Knowledge Base Management
- **Tools:** Markdown, Git, Static Site Generators, API Documentation Tools, Diagram Tools
- **Common Roles:** Technical Writer, Documentation Engineer, Developer Advocate, Product Manager

---

## Practical Guide to Technical Writing

### 1. Core Principles

**Clarity Over Cleverness**
- **Bad:** \"Leverage the synergistic potential of our multi-modal interface\"
- **Good:** \"Use the dashboard to view all your data in one place\"

**Audience Awareness**
- **Novice Users:** Step-by-step instructions with screenshots
- **Developers:** API references with code examples
- **Administrators:** Configuration guides with troubleshooting

**Accuracy First**
- Always test procedures yourself
- Document exact versions and system requirements
- Include error messages and recovery steps

### 2. Document Types & Structures

**API Documentation**
```markdown
# createUser

## Endpoint
`POST /api/v1/users`

## Parameters
| Name | Type | Required | Description |
|------|------|----------|-------------|
| email | string | Yes | Valid email address |
| role | enum | No | \"admin\" or \"user\" (default: \"user\") |

## Example Request
```json
{
  \"email\": \"user@example.com\",
  \"role\": \"admin\"
}
```

## Response
**Success (201 Created)**
```json
{
  \"id\": \"usr_123\",
  \"email\": \"user@example.com\",
  \"created_at\": \"2024-01-15T10:30:00Z\"
}
```

**Error (400 Bad Request)**
```json
{
  \"error\": \"Invalid email format\"
}
```
```

**Tutorial Structure**
1. **Objective:** What the user will accomplish
2. **Prerequisites:** Required knowledge and tools
3. **Steps:** Numbered, testable actions
4. **"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":22,"completion_tokens":450,"total_tokens":472,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":22},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
