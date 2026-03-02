# 🎵 Music Bingo App

A real-time Music Bingo application built with React, Node.js, Express, Socket.io, and Supabase.

## Project Structure

```
music-bingo-app/
├── server/              # Node.js/Express backend
│   ├── index.js         # Main server file with Socket.io
│   └── package.json     # Server dependencies
├── client/              # React frontend
│   ├── src/
│   │   └── App.js       # Main React component with bingo grid
│   └── package.json     # Client dependencies
├── .env                 # Environment variables
└── README.md            # This file
```

## Setup Instructions

### 1. Install Dependencies

**Server:**
```bash
cd server
npm install
```

**Client:**
```bash
cd client
npm install
```

### 2. Configure Environment Variables

Create/update the `.env` file in the root directory with your Supabase credentials:

```
SUPABASE_URL=your_supabase_url_here
SUPABASE_KEY=your_supabase_key_here
PORT=3001
```

Get these from your [Supabase project settings](https://app.supabase.com).

## Running the Application

### Terminal 1 - Start the Server

```bash
cd server
npm start
```

The server will run on `http://localhost:3001`

For development with auto-reload:
```bash
npm run dev
```

### Terminal 2 - Start the Client

```bash
cd client
npm start
```

The client will open at `http://localhost:3000` and automatically connect to the server.

## Features

- ✅ Real-time socket connection between client and server
- ✅ Bingo board generation
- ✅ Live updates via Socket.io
- ✅ Supabase integration for data persistence
- ✅ React-based UI with responsive grid

## Technologies Used

**Server:**
- Node.js
- Express
- Socket.io
- Supabase
- dotenv
- CORS

**Client:**
- React
- Socket.io Client
- Lucide React (icons)

## Development

To add new features:

1. **Server:** Modify `server/index.js` to add Socket.io event handlers
2. **Client:** Modify `client/src/App.js` to add UI components and Socket.io listeners

## License

MIT