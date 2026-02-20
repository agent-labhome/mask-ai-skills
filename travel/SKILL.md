-e # Travel

{"id":"2dcd2217-bf17-404d-b5ad-644d469a3657","object":"chat.completion","created":1771572503,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL.md: Travel Brief

## Skill Purpose
Generate concise, structured travel briefs based on user-provided trip details. Transforms scattered travel information into organized, actionable summaries.

## Core Functionality
- **Input Processing**: Accepts trip details in any format (paragraphs, bullet points, fragments)
- **Information Extraction**: Identifies key travel components (destinations, dates, accommodations, activities)
- **Structured Output**: Organizes information into standardized categories
- **Clarification**: Requests missing essential information when needed

## Input Requirements
Users should provide:
- Destination(s) and travel dates
- Accommodation details (if known)
- Planned activities or purpose
- Travel companions
- Budget considerations (optional)
- Special requirements (optional)

## Output Format
Always returns a markdown-formatted brief with these sections:

### 🧳 Trip Overview
- **Destination**: [Primary location]
