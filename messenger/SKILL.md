-e # Messenger

{"id":"0d95326f-9c23-46da-ae5a-23ca86a274c1","object":"chat.completion","created":1771578115,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Messenger - SKILL.md

## Core Functionality
Send and receive messages between users in real-time.

## Key Features
- **Direct Messaging**: One-on-one private conversations
- **Group Chats**: Multi-user conversations with shared messaging
- **Real-time Updates**: Instant message delivery and read receipts
- **Media Support**: Send images, files, and other attachments
- **Message History**: Access to past conversations

## User Flow
1. User selects a contact or group
2. Types message in chat input field
3. Sends message (Enter key or send button)
4. Message appears in conversation thread
5. Recipient receives notification and can reply

## Technical Requirements
- Real-time WebSocket/SSE connection for live updates
- Message persistence in database
- Push notifications for new messages
- File upload/storage for attachments
- User presence/typing indicators
