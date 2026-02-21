# Next.js SKILL.md

## Core Concepts
- **App Router** - File-based routing with `app/` directory (Next.js 13+)
- **Server Components** - Default: components render on server, reduce client JS
- **Client Components** - Use `"use client"` directive for interactivity
- **Server Actions** - Direct server functions from client components

## Key Features
- **SSR/SSG/ISR** - Multiple rendering strategies
- **Image Optimization** - Automatic with `next/image`
- **API Routes** - Backend endpoints in `app/api/` or `pages/api/`
- **Middleware** - Run code before requests (auth, redirects)

## Quick Commands
```bash
npx create-next-app@latest
npm run dev          # Development
npm run build        # Production build
npm start            # Run production
```

## Essential Patterns
```jsx
// Dynamic routes:"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":16,"completion_tokens":200,"total_tokens":216,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":16},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache