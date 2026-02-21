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