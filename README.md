Price Alert Bot (n8n Workflow): 
This n8n workflow monitors BTC/USDT price and sends Telegram alerts when the price exceeds a set threshold.

Workflow Diagram:

⏰ Schedule Trigger (every 2 min)
   ↓
🌐 HTTP Request (BTC/USDT price)
   ↓
🔎 If (price > 114,000 USDT)
   ↓
📲 Telegram Alert (send message)

Features:
Automated price checks every 2 minutes
Fetches BTC/USDT price from Finnhub
Sends Telegram alerts if price is above 114,000 USDT

Setup:
Import My workflow.json into n8n.
Configure your Telegram credentials.
Activate the workflow.

Customization"
Change the price threshold in the "If" node.
Update the Telegram chat ID.
Adjust the schedule interval.
License
MIT
