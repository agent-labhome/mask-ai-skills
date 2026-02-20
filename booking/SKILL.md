-e # Booking

{"id":"7ee8ac18-d4fe-4b52-b4c2-26d955e92301","object":"chat.completion","created":1771572523,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL: Booking

## Overview
The Booking skill enables users to schedule appointments, make reservations, or book services through natural language conversation. This skill handles date/time selection, service specification, participant details, and confirmation workflows.

## Core Capabilities

### 1. **Intent Recognition**
- Identify booking-related requests:
  - \"Book a table for dinner\"
  - \"Schedule a meeting with John\"
  - \"Reserve a conference room\"
  - \"Make a dental appointment\"
  - \"Book two tickets for the concert\"

### 2. **Slot Extraction**
Extract and validate:
- **Date/Time**: \"tomorrow at 3 PM\", \"next Monday\", \"December 25th\"
- **Service Type**: \"haircut\", \"massage\", \"consultation\"
- **Participants**: number of people, specific names
- **Location**: \"downtown branch\", \"main conference room\"
- **Duration**: \"1 hour\", \"30"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":14,"completion_tokens":200,"total_tokens":214,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":14},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
