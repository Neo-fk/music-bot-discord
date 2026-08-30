# 🎵 Music Bot for Discord

> ⚠️ **[ARCHIVED]** This project is **no longer actively maintained** and has been archived. This repository is kept for historical/educational purposes only. For production use, consider using actively maintained alternatives.

A feature-rich Discord music bot with intuitive button-based controls. Stream high-quality audio from YouTube directly in your Discord server with a seamless user experience.

---

## ✨ Features

- **Button-Based Controls** - Intuitive button interface for all music operations
- **High-Quality Playback** - Stream premium quality audio from YouTube
- **Queue Management** - Add, remove, and manage songs in the playlist
- **Loop Modes** - Support for loop one and loop all functionality
- **Volume Control** - Adjust playback volume on the fly
- **Now Playing Info** - Display current track and queue status
- **Skip & Stop** - Quick navigation through your playlist
- **Search Functionality** - Find and play songs directly from Discord
- **Server Support** - Works across multiple Discord servers

---

## 📋 Requirements

- **Node.js** v14.0 or higher
- **Discord.js** v13+
- **YouTube API Key** (for song search and playback)
- **Discord Bot Token** (from Discord Developer Portal)
- **FFmpeg** (for audio processing)

---

## 🚀 Installation

### Step 1: Clone the Repository
```bash
git clone https://github.com/Neo-fk/music-bot-discord.git
cd music-bot-discord
```

### Step 2: Install Dependencies
```bash
npm install
```

### Step 3: Configuration
1. **Create a `.env` file** in the root directory:
   ```env
   TOKEN=your_discord_bot_token_here
   ```

2. **Update `config.json`** with your server settings:
   ```json
   {
     "prefix": "!",
     "language": "en",
     "defaultVolume": 100
   }
   ```

3. **Add your YouTube API Key** in `config.js`:
   ```javascript
   const YOUTUBE_API_KEY = "your_youtube_api_key_here";
   ```

### Step 4: Run the Bot
```bash
node index.js
```

---

## 🎮 Usage

### Available Commands

| Command | Description |
|---------|-------------|
| `/help` | Display all available commands |
| `/play [song name]` | Play a song from YouTube |
| `/pause` | Pause current playback |
| `/resume` | Resume paused track |
| `/skip` | Skip to next song |
| `/skipall` | Clear queue and stop |
| `/stop` | Stop playback and leave voice channel |
| `/queue` | Show current playlist |
| `/remove [position]` | Remove song from queue |
| `/nowplaying` | Display current track info |
| `/loop` | Toggle loop mode |
| `/volume [level]` | Set volume (0-100) |
| `/join` | Join voice channel |
| `/leave` | Leave voice channel |
| `/invite` | Get bot invite link |

---

## 📁 Project Structure

```
music-bot-discord/
├── commands/
│   ├── Info/
│   │   ├── help.js
│   │   └── invite.js
│   └── music/
│       ├── join.js
│       ├── leave.js
│       ├── loop.js
│       ├── nowplaying.js
│       ├── pause.js
│       ├── play.js
│       ├── queue.js
│       ├── remove.js
│       ├── resume.js
│       ├── search.js
│       ├── skip.js
│       ├── skipall.js
│       ├── stop.js
│       └── volume.js
├── handlers/
│   └── command.js
├── JSON/
│   └── ad.json
├── config.js
├── config.json
├── index.js
├── package.json
└── README.md
```

---

## 🔧 Setup Guide

### Discord Developer Portal

1. Visit [Discord Developer Portal](https://discord.com/developers/applications)
2. Click **"New Application"** and name your bot
3. Navigate to **"Bot"** tab and click **"Add Bot"**
4. Under **TOKEN**, click **"Copy"** to copy your bot token
5. Paste the token in your `.env` file

### YouTube API Key

1. Visit [Google Cloud Console](https://console.cloud.google.com)
2. Create a new project
3. Enable **YouTube Data API v3**
4. Create a credential (API Key)
5. Add the key to `config.js`

### Inviting the Bot

1. Go to **OAuth2** → **URL Generator** in Developer Portal
2. Select scopes: `bot`
3. Select permissions: 
   - Read Messages/View Channels
   - Send Messages
   - Connect (to voice)
   - Speak
4. Use the generated URL to invite the bot to your server

---

## 🐳 Deployment Options

### Replit

[![Run on Repl.it](https://repl.it/badge/github/Neo-fk/music-bot-discord)](https://replit.com/@FbTo/music-bot-discord-1?v=1)

### Local Machine
```bash
npm install
node index.js
```

### Docker (Optional)
Create a `Dockerfile` for containerized deployment.

---

## 📸 Screenshots

**Now Playing Interface:**
![play](https://i.ibb.co/pfRqHXK/Screenshot-42.png)

**Help Command:**
![help](https://i.ibb.co/ZgM0kVD/Screenshot-43.png)

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⚠️ Disclaimer

This bot is designed for educational purposes. Ensure compliance with Discord's Terms of Service and YouTube's API usage policies when deploying.

---

## 📧 Support

For issues, questions, or suggestions, please open an [Issue](https://github.com/Neo-fk/music-bot-discord/issues) on GitHub.

---

**Made with ❤️ by [Neo-fk](https://github.com/Neo-fk)**
