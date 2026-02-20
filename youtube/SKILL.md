-e # YouTube

{"id":"6f079dfa-dedc-4cfd-8a85-4904f782bc18","object":"chat.completion","created":1771585544,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL.md: YouTube

## Core Functionality
- Search and play YouTube videos directly in chat
- Retrieve video details (title, duration, views, uploader)
- Provide video summaries and key information
- Handle YouTube URLs and search queries

## Supported Commands & Queries
- \"Play [song/video name] on YouTube\"
- \"Search YouTube for [topic]\"
- Direct YouTube URLs (youtube.com/watch?v=...)
- \"Show me videos about [subject]\"
- \"YouTube video [title]\"

## Technical Notes
- Returns video metadata without embedding actual players
- Provides clickable links to YouTube
- Can summarize video content when available
- Respects YouTube's terms of service

## Limitations
- No video downloading capability
- No playback within chat interface
- Limited to publicly available videos
