# 📈 Price Alert Bot (n8n Workflow)

This **n8n workflow** monitors the **BTC/USDT** price in real-time and sends a **Telegram alert** when the price exceeds a set threshold.

---

## 📊 Workflow Diagram
⏰ Schedule Trigger (every 2 min)
↓
🌐 HTTP Request (BTC/USDT price from Finnhub)
↓
🔎 If (price > 114,000 USDT)
↓
📲 Telegram Alert (send message)


---

## 🚀 Features
- ⏱ **Automated checks** every 2 minutes  
- 🌐 **Fetches BTC/USDT price** from [Finnhub API](https://finnhub.io)  
- 📢 **Sends Telegram alerts** when the price is above your chosen threshold  

---

## ⚙️ Setup Instructions

### 1️⃣ Import the Workflow
- Download the `workflow.json` file.
- Open your **n8n dashboard**.
- Go to **Workflows → Import from File** and select `workflow.json`.

### 2️⃣ Configure API & Telegram Credentials
- **Finnhub API Key**:  
  - Sign up at [Finnhub](https://finnhub.io) and get your API key.
  - In the **HTTP Request** node, replace `YOUR_API_KEY` with your key.
- **Telegram Credentials**:  
  - Create a bot with [BotFather](https://core.telegram.org/bots#6-botfather).
  - Get your `BOT_TOKEN` and add it to the **Telegram node**.
  - Replace the `chat_id` with your own.

### 3️⃣ Activate the Workflow
- Click **Activate** to start monitoring prices.

---

## 🔧 Customization
- **Change Price Threshold**:  
  - Open the **If node** and update the condition `(price > 114000)`.
- **Adjust Schedule Interval**:  
  - Edit the **Cron node** to run at your preferred frequency.
- **Change Currency Pair**:  
  - Update the Finnhub API request URL to track other symbols (e.g., ETH/USDT).

---

## 📜 License
This project is licensed under the **MIT License** — you are free to use, modify, and distribute.

---


