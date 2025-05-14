# MicronutrientBot – Setup Guide


## Prerequisites
- Python 3.8+
- [Ngrok](https://ngrok.com/) (for local tunneling)
- Dialogflow Essentials account

## Setup Instructions

### 1. Import Dialogflow Agent
1. Unzip the provided `MicronutrientBot_Agent_sub` to access the Dialogflow agent files
2. Navigate to the [Dialogflow Console](https://dialogflow.cloud.google.com/)
3. Create a new agent (or use an existing one)
4. Click the  Settings icon → Export & Import → Restore from ZIP
5. Upload the agent ZIP file to gain access to the agent 

### 2. Configure Flask Backend
1. Unzip the Flask webhook code 
2. Install flask, Ngrok and Python 3.8+

 3. Run Locally with Ngrok
1. Start Ngrok (to expose your local server) by running: ngrok http 5000
   Copy the HTTPS URL that appears (e.g., https://abc123.ngrok.io)
2. In Dialogflow:
   - Go to Fulfillment → Enable Webhook
   - Paste your Ngrok URL (e.g., https://abc123.ngrok.io/webhook)
3. Run the Flask app by executing: python app.py

## Running the bot
1. Use the Dialogflow test console or the integrated web interface by typing in broswer local host:8080

