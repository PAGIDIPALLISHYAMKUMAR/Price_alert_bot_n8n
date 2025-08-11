Price Alert Bot (n8n Workflow)
This project is an n8n workflow that monitors the price of BTC/USDT using the Finnhub API and sends a Telegram alert when the price exceeds a specified threshold.

Features:
Scheduled price checks every 2 minutes
Fetches BTC/USDT price from Finnhub
Sends Telegram alerts when price is above 114,000 USDT


Workflow Overview:
Schedule Trigger: Runs every 2 minutes.
HTTP Request: Fetches the latest BTC/USDT price from Finnhub.
If Condition: Checks if the price (c field) is greater than 114,000 USDT.
Telegram Message: Sends an alert to the specified Telegram chat.


Setup:
Clone this repository or copy the workflow JSON.
Import My workflow.json into your n8n instance.
Set up your Telegram credentials in n8n.
Activate the workflow.


Customization:
Change the price threshold in the "If" node.
Update the Telegram chat ID in the "Send a text message" node.
Adjust the schedule interval as needed.
