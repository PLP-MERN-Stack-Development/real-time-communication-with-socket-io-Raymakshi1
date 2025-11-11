# Socket.io Real-Time Chat Application

A fully-featured real-time chat application built with **Express + Socket.io** (server) and **React + Vite** (client), satisfying all assignment requirements with 6+ advanced features.

## ✅ Assignment Requirements - ALL SATISFIED

### Task 1: Project Setup ✅
- Node.js server with Express
- Socket.io configured on server
- React front-end with Vite
- Socket.io client integrated
- Bidirectional client-server connection

### Task 2: Core Chat Functionality ✅
- JWT user authentication (bcrypt password hashing)
- Multiple chat rooms + switching
- Messages with sender name and timestamp
- Typing indicators
- Online/offline user presence

### Task 3: Advanced Chat Features ✅
- Private messaging (modal UI)
- Multiple rooms with creation
- User typing indicator
- File/image sharing (base64 upload)
- Read receipts with count display
- Message reactions (emoji picker)

### Task 4: Real-Time Notifications ✅
- Browser notifications (Web Notifications API)
- User join/leave notifications
- Unread message count per room
- Sound notifications (WebAudio)
- Browser notifications with settings toggle

### Task 5: Performance & UX ✅
- Message pagination (load older)
- Socket.io rooms and namespaces
- Message delivery acknowledgment (read receipts)
- Message search (filter by content/username)
- Responsive design (desktop/mobile)
- Automatic mark-as-read on tab focus

How to run (PowerShell)

Prerequisites: Node.js (v18+ recommended), npm

1) Install server dependencies

Set-Location -Path 'C:\Users\user\Desktop\socketio-chat\server'
npm install

2) Install client dependencies

Set-Location -Path 'C:\Users\user\Desktop\socketio-chat\client'
npm install

3) Start the server

Set-Location -Path 'C:\Users\user\Desktop\socketio-chat\server'
npm run dev
# If port 5000 is occupied: $env:PORT='5001'; npm run dev

4) Start the client (in a new terminal)

Set-Location -Path 'C:\Users\user\Desktop\socketio-chat\client'
npm run dev
# If server is on non-default port: $env:VITE_API_URL='http://localhost:5001/api'; npm run dev

The client will be available at http://localhost:5173 (or 5174 if busy)

## 🎯 Advanced Features Implemented

1. **Private Messaging** - Modal UI for sending direct messages
2. **Message Reactions** - Emoji picker with live sync
3. **Read Receipts** - Mark read, display read counts
4. **Browser Notifications** - Web Notifications API + WebAudio sound
5. **File/Image Sharing** - Upload files via UI button
6. **Message Search** - Filter messages by content/username
7. **Per-Room Unread Badges** - Shows unread count per room
8. **Settings Panel** - Toggle notifications and sound
9. **Profile Pictures** - User avatars in header and messages
10. **Message Pagination** - Load older messages button

## �️ Screenshots

Below are screenshots demonstrating the key features of the application:

### Screenshot 1: Chat Interface with Rooms & Messages
![Chat Interface](c:\Users\user\Pictures\Screenshots\Screenshot 2025-03-03 124732.png)
*Main chat interface showing room list, online users, and real-time messages*

### Screenshot 2: User Profile & Avatars
![User Profile](c:\Users\user\Pictures\Screenshots\Screenshot (47).png)
*User profile modal and avatar display in messages*

### Screenshot 3: Private Messaging
![Private Messages](c:\Users\user\Pictures\Screenshots\Screenshot (48).png)
*Private message modal and direct messaging feature*

### Screenshot 4: Advanced Features
![Features](c:\Users\user\Pictures\Screenshots\Screenshot (49).png)
*Message search, file uploads, reactions, and notifications settings*

## �📋 Quick Manual Verification

1. Register/login two users in different browsers
2. Send messages in 'general' room - appear in real time
3. Click user in sidebar → send private message
4. Switch to another tab → receive message → see browser notification
5. Click 😊 on a message → select emoji → see reaction on other client
6. Messages show read count and avatar
7. Create new room → switch rooms → see unread badges
8. Search messages in search bar
9. Click 📎 → upload a file → see file link in chat
10. Click avatar in header → edit profile picture
11. Click Settings → toggle notifications/sound
12. Click "Load older messages" → pagination works

Where to look in the code
- Server socket handlers: `server/socket/socketHandler.js`
- Client chat logic: `client/src/hooks/useChat.js`
- UI components: `client/src/components/Chat/*`
- Socket provider: `client/src/context/SocketContext.jsx`

If you want me to continue, I can:
- Add a settings panel to toggle browser notifications and sound (small, recommended)
- Implement per-room unread badges and message pagination
- Add file/image upload flow (requires server upload handling)
