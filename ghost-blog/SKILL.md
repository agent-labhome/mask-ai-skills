-e # Ghost Blog

{"id":"1f0b1d52-8a3c-4d78-bd4e-6346913cdb89","object":"chat.completion","created":1771516145,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Ghost Blog SKILL.md

## Purpose
Quickly create and manage blog posts in Ghost CMS via CLI.

## Commands
- `ghost post \"Title\"` – Create new draft post
- `ghost list` – Show recent posts (drafts/published)
- `ghost publish [id]` – Publish a draft
- `ghost update [id] \"New title\"` – Update post title
- `ghost delete [id]` – Delete a post

## Setup
1. Get Ghost Admin API key from Settings → Integrations
2. Set environment variable: `GHOST_API_URL` and `GHOST_ADMIN_API_KEY`

## Notes
- Works with Ghost 5.x+
- All posts created as drafts by default
- Use numeric IDs from `ghost list` for updates/deletion"},"logprobs":null,"finish_reason":"stop"}],"usage":{"prompt_tokens":16,"completion_tokens":176,"total_tokens":192,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":16},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
