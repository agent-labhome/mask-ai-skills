## Core Concepts
- **App Router** - File-based routing with `app/` directory
- **Server Components** - Default (no 'use client'), run on server
- **Client Components** - Add 'use client' directive for interactivity
- **Server Actions** - Direct server mutations from client components

## Key Patterns
- Use `async` Server Components for data fetching
- Implement loading states with `loading.js`
- Handle errors with `error.js`
- Add metadata in `layout.js` or `page.js`
- Use `generateStaticParams` for static generation

## Performance
- Automatic code splitting
- Image optimization via `next/image`
- Font optimization with `next/font`
- Streaming and Suspense for progressive loading

## Quick Start
```bash
npx create-next-app@latest
```