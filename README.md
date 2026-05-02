💸CorpEvent Tracker💸

## 📌 Overview
A real-time automation system that tracks NSE corporate board meetings and sends alerts via Telegram.

## ❗ Problem
Investors often miss important corporate announcements like board meetings, earnings, and strategic decisions because data is scattered and not actively tracked.

## 💡 Solution
This system automates the tracking of board meeting data using APIs and sends real-time alerts, ensuring investors never miss key events.

## ⚙️ How It Works
1. Fetch stock list from Google Sheets  (must be symbols from NSE)
2. Filter out non-relevant instruments (ETF, IPO, etc.)  
3. Call NSE API for board meeting data  
4. Detect new events  
5. Check duplicates using Google Calendar  
6. Create event + send Telegram alert  

Flow:
Google Sheets(holdings source) → n8n → NSE API → Calendar → Telegram

## 🔧 Tech Stack
- n8n (workflow automation)
- NSE API (data source)
- Google Sheets (input data)
- Google Calendar (deduplication + storage)
- Telegram Bot API (alerts)

## 📊 Features
- Real-time board meeting tracking  
- Duplicate detection system  
- Automated calendar logging  
- Instant Telegram alerts  
- Scheduled execution (multiple times per day)  

## 🚀 Setup Instructions
1. Import `workflow.json` into n8n  
2. Connect Google Sheets + Calendar  
3. Add Telegram bot credentials  
4. Run workflow   

## 🤝 Use Case
Built for:
- Retail investors  
- Swing traders  
- Finance enthusiasts  

## 🧑‍💻 Author
cv-yethin
