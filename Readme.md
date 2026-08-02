<div align="center">

<img src="https://i.ibb.co/cKzySsgr/yy.png" alt="Mandir Music" width="400"/>

# 🎵 ˹Mᴀɴᴅɪʀ 𝙼𝚞𝚜𝚒𝚌˼

### A Modern Telegram Music Bot for High-Quality Voice Chat Streaming

An open-source Telegram music bot built with **Python**, **Pyrogram**, **PyTgCalls**, and **FFmpeg**, delivering fast, reliable, and high-quality audio streaming directly to Telegram voice chats.

<br>

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/hasindu-nagolla/MandirMusicBot?style=for-the-badge)](https://github.com/hasindu-nagolla/MandirMusicBot/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/hasindu-nagolla/MandirMusicBot?style=for-the-badge)](https://github.com/hasindu-nagolla/MandirMusicBot/network/members)
[![GitHub Issues](https://img.shields.io/github/issues/hasindu-nagolla/MandirMusicBot?style=for-the-badge)](https://github.com/hasindu-nagolla/MandirMusicBot/issues)

[![Telegram Channel](https://img.shields.io/badge/Telegram-Channel-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/TheInfinityAI)
[![Telegram Support](https://img.shields.io/badge/Telegram-Support-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/Hasindu_Lakshan)

</div>

---

## 📖 About

**˹Mᴀɴᴅɪʀ 𝙼𝚞𝚜𝚒𝚌˼** is a powerful and modern Telegram music bot built for seamless voice chat streaming. It enables users to play music directly in Telegram voice chats using YouTube links, search queries, and live radio stations while offering administrators complete control over playback.

Designed with performance, stability, and simplicity in mind, the project combines modern asynchronous technologies to provide a fast, reliable, and highly customizable music streaming experience. Whether you're hosting a small community or managing a large Telegram group, Mandir Music is built to deliver consistent performance with minimal configuration.

---

# 📑 Table of Contents

- [📖 About](#-about)
- [⭐ Why Mandir Music?](#-why-mandir-music)
- [✨ Features](#-features)
- [🏗 Tech Stack](#-tech-stack)
- [📋 Requirements](#-requirements)
- [🚀 Quick Start](#-quick-start)
- [⚙️ Environment Variables](#️-environment-variables)
- [🛠 Installation](#️-installation)
- [📖 Commands](#-commands)
- [📂 Project Structure](#-project-structure)
- [🤝 Contributing](#-contributing)
- [📞 Support](#-support)
- [🙏 Credits](#-credits)
- [📄 License](#-license)

---

# ⭐ Why Mandir Music?

Choosing the right Telegram music bot shouldn't mean sacrificing performance, reliability, or ease of deployment. Mandir Music is designed with developers and communities in mind, providing a clean architecture, modern technologies, and powerful features while remaining simple to deploy and maintain.

### Highlights

- 🚀 Fast and lightweight architecture
- 🎵 High-quality voice chat streaming
- 🎧 YouTube search and direct URL playback
- 📻 Built-in live radio support
- 📝 Smart queue management
- 🛡 Powerful administrator controls
- 👥 User authorization system
- 🔄 Automatic voice chat cleanup
- 🐳 Docker and Docker Compose support
- ⚙️ Environment-based configuration
- 📂 Modular and maintainable codebase
- ❤️ Open-source under the GPL-3.0 License

---

# ✨ Features

### 🎵 High-Quality Audio Streaming

Experience smooth and crystal-clear music playback optimized for Telegram voice chats using the Opus codec and FFmpeg.

### 🎧 YouTube Integration

Play music instantly from:

- YouTube links
- Search queries
- Supported playlists

### 📻 Live Radio Streaming

Access and stream a collection of online radio stations directly within Telegram voice chats.

### 📝 Smart Queue Management

Manage playlists effortlessly with a built-in queue system.

- Add songs
- View queue
- Skip tracks
- Clear queue

### ⚡ Optimized Performance

Built with asynchronous libraries for efficient resource usage and responsive performance.

### 🎛 Playback Controls

Complete playback management with support for:

- Play
- Pause
- Resume
- Skip
- Stop
- Seek

### 👥 Authorization System

Restrict playback controls to:

- Chat administrators
- Authorized users
- Bot owner
- Sudo users

### 🔄 Automatic Voice Chat Cleanup

Automatically detects inactive voice chats and leaves them to conserve server resources.

### 🐳 Docker Ready

Deploy effortlessly using Docker or Docker Compose for a consistent production environment.

### 🔧 Easy Configuration

Configure the bot entirely through environment variables without modifying the source code.

---

# 🏗 Tech Stack

| Category | Technology |
|-----------|------------|
| Language | Python 3.10+ |
| Telegram Framework | Pyrogram |
| Voice Chat | PyTgCalls |
| Database | MongoDB |
| Media Processing | FFmpeg |
| Runtime | Deno & Ballerina |
| Containerization | Docker & Docker Compose |
| Version Control | Git |

---

# 📋 Requirements

Before deploying **˹Mᴀɴᴅɪʀ 𝙼𝚞𝚜𝚒𝚌˼**, ensure your system meets the following requirements.

| Software | Version |
|-----------|---------|
| Python | 3.10 or higher |
| FFmpeg | Latest |
| Deno | Latest |
| Ballerina | 2201.9.0 (Swan Lake) or higher |
| MongoDB | Atlas or Self-hosted |
| Git | Latest |

### 🔧 Installing Prerequisites (Linux/Ubuntu)

Before starting, install the required runtimes:

```bash
# Install FFmpeg
sudo apt update && sudo apt install ffmpeg -y

# Install Deno
curl -fsSL https://deno.land/x/install/install.sh | sh

# Install Ballerina (Swan Lake)
wget -O ballerina.deb https://dist.ballerina.io/downloads/2201.9.0/ballerina-2201.9.0-swan-lake-linux-x64.deb
sudo dpkg -i ballerina.deb
```

---

# 🚀 Quick Start

Clone the repository.

```bash
git clone https://github.com/hasindu-nagolla/MandirMusicBot.git
```

Move into the project directory.

```bash
cd MandirMusicBot
```

Install the required dependencies.

```bash
pip install -r requirements.txt
```

Create your environment configuration.

```bash
cp sample.env .env
```

Update the values inside `.env`.

Start the Ballerina microservice API in a background session (e.g., using `tmux`).

```bash
tmux new -s StatsAPI
bal run stats_api.bal
# Detach the session using Ctrl+B then D
```

Start the bot in another session.

```bash
bash start
```

---

# ⚙️ Environment Variables

Create a `.env` file in the project's root directory.

```env
# Telegram API
API_ID= 33466543
API_HASH= a196bb5a620eb6f06131956416bee22f
BOT_TOKEN= 8807013740:AAEbzGyzes0XYj-5QlBC7LyoVLQAyDUmK68

# MongoDB
MONGO_DB_URI= mongodb+srv://chichibbe9122006_db_user:sohpWhPbZHnDBl3G@cluster0.qucbfub.mongodb.net/?appName=Cluster0

# Bot Configuration
OWNER_ID= 5858663864
LOGGER_ID= -1004405423450

# Assistant Account
STRING_SESSION=BQH-qK8AazH2c6LC8P9yTviyyTdKwRKu9fO9Z4YkmHcqpnv2yj4YgA10jnLD7emtR4ztq2BpPnIyVLIyyCbrXkIrnq_YW3SGl2YpirOfLAtjbkw1pKlmqUv1yGylzDeN-WJauMdyKlBb1edAJ810UhlFpO-43dFt5QteqZSxloXlm_RmR1wBrV-Z7Br5mInoTBhZajw5j0YTsbfTp9jZu5afeY2egq5hzukej9i2Ce_OVf8CqcG3kuWy0nBFuzww56DjAFMoAM8aLAMjBDigkIoadwtRlWbTJ-wWeg70CD8OrWEFN9HAw2V97nUx81JaMMfBRuaOyzUZDUOZUD8LOrS-Lug8lgAAAAIIFOJuAA

# Essential
COOKIE_URL=COOKIE_URL=https://batbin.me/raw/traumatologies
```

| Variable | Description |
|-----------|-------------|
| `API_ID` | Telegram API ID obtained from **my.telegram.org** |
| `API_HASH` | Telegram API Hash |
| `BOT_TOKEN` | Bot Token received from **@BotFather** |
| `MONGO_DB_URI` | MongoDB connection URI |
| `OWNER_ID` | Telegram User ID of the bot owner |
| `LOGGER_ID` | Group ID used for bot logs |
| `STRING_SESSION` | Pyrogram String Session for the assistant account |
| `COOKIE_URL` | YouTube cookies URL |

---

# 🛠 Installation

## Local Installation

Clone the repository.

```bash
git clone https://github.com/hasindu-nagolla/MandirMusicBot.git
```

Enter the project directory.

```bash
cd MandirMusicBot
```

Install Python dependencies.

```bash
pip install -r requirements.txt
```

Create the environment file.

```bash
cp sample.env .env
```

Configure all required environment variables.

Start the Ballerina microservice API in a background session.

```bash
tmux new -s StatsAPI
bal run stats_api.bal
# Detach the session using Ctrl+B then D
```

Start the bot.

```bash
bash start
```

---

## Docker

Build the Docker image.

```bash
docker build -t mandirmusicbot:latest .
```

Run the container.

```bash
docker run -d \
  --restart unless-stopped \
  --env-file .env \
  -v ./MandirMusic/cookies:/app/MandirMusic/cookies \
  -v ./downloads:/app/downloads \
  --name mandirmusicbot \
  mandirmusicbot:latest
```

---

## Docker Compose

Deploy using Docker Compose.

```bash
docker compose up -d --build
```

View container logs.

```bash
docker compose logs -f
```

Stop the services.

```bash
docker compose down
```

Restart the services.

```bash
docker compose restart
```

---

# 📖 Commands

## 👤 User Commands

| Command | Description |
|---------|-------------|
| `/play <song/url>` | Play a song from a YouTube URL or search query |
| `/radio` | Browse available radio stations |
| `/queue` | Display the current music queue |
| `/ping` | Check the bot's latency and status |
| `/help` | Show the help menu |

---

## 🛡 Admin Commands

| Command | Description |
|---------|-------------|
| `/pause` | Pause the current playback |
| `/resume` | Resume playback |
| `/skip` | Skip the current track |
| `/next` | Play the next track in the queue |
| `/stop` | Stop playback |
| `/end` | Stop playback and clear the queue |
| `/seek <time>` | Seek to a specific timestamp |
| `/reload` | Reload administrator cache |

---

## 👑 Owner Commands

| Command | Description |
|---------|-------------|
| `/stats` | Display bot statistics |
| `/broadcast` | Broadcast a message to all served chats |
| `/addsudo` | Add a sudo user |
| `/rmsudo` | Remove a sudo user |

| `/maintenance` | Enable or disable maintenance mode |
| `/restart` | Restart the bot |
| `/logs` | Retrieve the latest bot logs |

---

# 📂 Project Structure

```text
MandirMusicBot/
├── MandirMusic/
│   ├── __init__.py
│   ├── __main__.py
│   ├── cookies/
│   ├── core/
│   ├── helpers/
│   ├── locales/
│   └── plugins/
│
├── config.py
├── sample.env
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── setup
├── start
├── LICENSE
└── Readme.md
```

---

# 🤝 Contributing

Contributions are welcome and greatly appreciated.

Whether you're fixing bugs, improving documentation, optimizing performance, or adding new features, your contributions help make **˹Mᴀɴᴅɪʀ 𝙼𝚞𝚜𝚒𝚌˼** better for everyone.

Please read the [CONTRIBUTING.md](CONTRIBUTING.md) guide before opening an issue or submitting a pull request.

---

# 📞 Support

Need help with deployment or encountered an issue?

Feel free to reach out through the following platforms.

| Platform | Link |
|----------|------|
| 💻 GitHub Repository | https://github.com/hasindu-nagolla/MandirMusicBot |
| 📢 Telegram Channel | https://t.me/Mandir_shop |
| 💬 Telegram Support | https://t.me/slot_by_rex |

If you discover a bug, please open a GitHub Issue with detailed information so it can be reproduced and fixed quickly.

---

# 🙏 Credits

This project would not have been possible without the amazing open-source community.

Special thanks to:

- **[Anony](https://github.com/AnonymousX1025)** — Inspiration for the original project.
- **[Pyrogram](https://github.com/pyrogram/pyrogram)** — Telegram MTProto framework.
- **[PyTgCalls](https://github.com/pytgcalls/pytgcalls)** — Telegram voice chat streaming library.
- **[FFmpeg](https://ffmpeg.org/)** — Audio processing and transcoding.

Thank you to everyone who has contributed through code, bug reports, feature suggestions, testing, and community support.

---

# 📄 License

This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.

You are free to use, modify, and distribute this software. However, any derivative works must also be open-source and released under the exact same license. 

For more information, see the [LICENSE](LICENSE) file.

---

<div align="center">

## ⭐ Support the Project

If you find **˹Mᴀɴᴅɪʀ 𝙼𝚞𝚜𝚒𝚌˼** useful, consider giving this repository a ⭐ on GitHub.

Your support helps increase the project's visibility and encourages future development.

<br>

**Made with ❤️ by <a href="https://github.com/hasindu-nagolla">Hasindu Nagolla</a>**

</div>
