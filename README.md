# Telegram Bot API Binaries (Automated Builds)

[![GitHub Release](https://img.shields.io/github/v/release/coyotle/telegram-bot-api-bin?include_prereleases&style=flat-square)](https://github.com/coyotle/telegram-bot-api-bin/releases)  
[![Build Status](https://img.shields.io/github/actions/workflow/status/coyotle/telegram-bot-api-bin/release-bot-api.yml?style=flat-square)](https://github.com/coyotle/telegram-bot-api-bin/actions)

Automated builds of **[Telegram Bot API](https://core.telegram.org/bots/api)** for Linux.  
New versions are published here within 24 hours of updates to the official [API Changelog](https://core.telegram.org/bots/api-changelog).

---

## 📦 Quick Start

### Download the Latest Binary

```bash
wget https://github.com/coyotle/telegram-bot-api-bin/releases/latest/download/telegram-bot-api
chmod +x telegram-bot-api
```

### Run the Server

```bash
./telegram-bot-api --local --http-port=8081 --verbosity=1
```

### Verify It Works

```bash
curl http://localhost:8081/api/v1/health
# Expected response: {"ok":true}
```

## 🔄 Versioning

Each release matches an official Bot API version (e.g., v6.9).

Binaries are rebuilt daily to ensure compatibility.

## 🛠 Build System

Built automatically via GitHub Actions using:

Source: tdlib/telegram-bot-api

Toolchain: CMake, GCC 11+, OpenSSL 3.0

Platforms: Linux/x86_64 (others available on request).

## 📜 License

This project distributes binaries under the same license as the original source.
