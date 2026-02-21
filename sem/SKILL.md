-e {"id":"13366bf3-3efe-4d26-8eb3-5c64ec2ff8dc","object":"chat.completion","created":1771649778,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL.md: Semantic Error Messages (SEM)

## Metadata
- **Skill Name**: Semantic Error Messages (SEM)
- **Version**: 1.0.0
- **Category**: Programming/Developer Tools
- **Author**: AI Assistant
- **Description**: Generates comprehensive, human-readable error messages with semantic context, debugging suggestions, and educational explanations
- **Tags**: debugging, error-handling, programming, education, developer-tools
- **Compatibility**: Language-agnostic, adaptable to multiple programming languages
- **License**: MIT

## Overview
SEM transforms cryptic error messages into meaningful, actionable insights. It analyzes error codes, stack traces, and context to provide:
- Plain English explanations
- Likely causes and solutions
- Code examples for fixes
- Prevention strategies
- Related documentation links

## Core Features

### 1. **Error Decoding**
- Parses technical error messages
- Identifies error patterns across languages
- Extracts relevant variables and line numbers
- Maps to common programming concepts

### 2. **Contextual Analysis**
- Considers surrounding code context
- Analyzes variable states and data flow
- Detects common anti-patterns
- Identifies language/framework-specific issues

### 3. **Solution Generation**
- Provides step-by-step fixes
- Offers multiple solution approaches
- Includes code snippets for correction
- Suggests debugging techniques

### 4. **Educational Content**
- Explains underlying concepts
- Links to relevant documentation
- Provides best practices
- Includes prevention strategies

## Usage Guide

### Basic Usage
```python
# Example: Python error analysis
error_message = \"TypeError: can only concatenate str (not 'int') to str\"
sem_response = analyze_error(error_message, context=current_code)
```

### Input Format
SEM accepts:
- Raw error messages
- Stack traces
- Code snippets with errors
- Runtime exception details
- Compiler output

### Output Structure
```json
{
  \"error_summary\": \"Human-readable summary\",
  \"root_cause\": \"Primary issue explanation\",
  \"immediate_fix\": \"Quick solution steps\",
  \"detailed_explanation\": \"Conceptual background\",
  \"code_examples\": {
    \"incorrect\": \"Buggy code example\",
    \"correct\": \"Fixed version\"
  },
  \"prevention_tips\": [\"Best practices\"],
  \""},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":18,"completion_tokens":500,"total_tokens":518,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":18},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
