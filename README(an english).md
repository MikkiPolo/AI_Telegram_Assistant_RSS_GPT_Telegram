# 🤖 AI Telegram Assistant: RSS → GPT → Telegram

This project is an AI-powered automation built with [Make.com (Integromat)](https://www.make.com/) that turns news from RSS feeds into personalized, media-rich posts for a Telegram channel — fully automated and styled with GPT-generated copy.

---

## 🔁 Workflow Overview

Every hour, the scenario:

1. **Watches RSS feed** for new items.
2. **Fetches the full article** via HTTP (from the link provided in the RSS).
3. **Extracts clean text** from the HTML content.
4. **Uses OpenAI (GPT-4)** to:
   - Generate a **short catchy headline**
   - Add a **commentary in the style of the Telegram channel author**
5. **Resizes image** from the RSS feed to meet Telegram’s media requirements.
6. **Publishes the final post** (text + image) directly to the Telegram channel via bot.

---

## 📦 Technologies Used

- [Make.com (Integromat)](https://www.make.com/) — no-code visual automation
- [OpenAI GPT-4](https://platform.openai.com/) — for text generation
- [Telegram Bot API](https://core.telegram.org/bots/api) — for posting content
- **RSS + HTTP + HTML Parser** — to fetch and clean article content
- **Image Resize module** — to ensure valid photo dimensions for Telegram

---

## 💡 Key Features

- 🎯 **Autopilot publishing**: runs every hour, no manual input required
- 🧠 **GPT-personalized tone**: customizable style for different niches (e.g. fashion, coaching, news)
- 🖼️ **Dynamic media support**: adds images when available and resizes them automatically
- ✍️ **Human-like Telegram copy**: short and catchy, feels like it’s written by a real person

---

## 📍 Example Use Cases

| Niche       | Purpose                                 |
|-------------|-----------------------------------------|
| Fashion     | Post industry news with styled comments |
| Coaching    | Share insights and trends automatically |
| Tech/Crypto | Summarize and share updates instantly   |
| Job Boards  | Turn listings into digestible summaries |

---

## ⚙️ Trigger & Logic

- **Trigger:** Automatic, every hour
- **Image Logic:** Only sends images if available and valid (resized via Make)
- **Text Logic:** All prompts and post structures handled via GPT

> 📌 _Prompt logic is confidential and not published in this repository._

---

## 📲 Output Example