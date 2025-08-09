# Jumping Spyder

## 🚀 Overview
**Jumping Spyder** is a JavaScript-powered Telegram bot for **Solana** traders.  
It delivers **real-time sentiment signals**, token tracking, and premium features unlocked via **on-chain SOL balance checks**.  

Built with [Telegraf](https://telegraf.js.org/) + Solana wallet integration, it’s designed for speed, simplicity, and trader-focused insights.  

---
**Hackathon Category**: Consumer Apps, DeFi

## ✨ Features

- **📥 Onboarding** – `/start` greets users with interactive inline buttons.  
- **📡 Live Signals** – `/getsignals` subscribes users to curated crypto alpha feeds.  
- **🔍 Token Tracking** – `/track_token` (e.g., `/track SOL`) for focused sentiment alerts.  
- **💬 Help & Feedback** – `/help` and `/feedback` for guidance & bug reports.  
- **⚙ Settings Preview** – `/settings` for upcoming customization options.  
- **💰 Premium Access via Solana Wallet** – `/subscribe` generates a **unique Solana public key** for each user, checks SOL balance, and unlocks premium features on deposit.  

---

## 📂 Key Files

- `jumping_spyder/bot.js` → Main Telegram bot commands & logic  
- `jumping_spyder/solana/paymentGate.js` → Deterministic Solana wallet generation & balance checks  

---

## 🛠 Usage

```bash
# 1️⃣ Install dependencies
npm install

# 2️⃣ Configure .env
# Fill in Telegram token, X API key, Solana mnemonic, etc.

# 3️⃣ Run the bot
node jumping_spyder/bot.js
🔑 Environment Variables
BOT_TOKEN → Telegram bot token

MNEMONIC → Solana wallet mnemonic

TELEGRAM_CHANNEL_ID → Target channel/user for alerts

(Optional) API keys for Twitter/OpenAI integrations

🎯 Example: Premium Unlock
When a user sends /subscribe:

A unique Solana public key is derived from their Telegram user ID.

SOL balance is checked on-chain.

Access is granted if balance meets premium threshold.

📜 License
MIT License © 2025 stef849 — All rights reserved for this modified version.
