# MicronutrientBot
CS3IP 
# MicronutrientBot – Setup Guide

This chatbot project uses Python (Flask) for the backend and Dialogflow Essentials for natural language processing. It allows users to ask nutrition-related questions and receive food suggestions based on symptoms, nutrients, and their personal profile.

Step 1: Set up Dialogflow Agent

1. Unzip the Dialogflow folder "MicronutrientBot-sub" in this project. Inside you’ll find a ZIP file of the agent

 2. Go to [Dialogflow Essentials Console]
    
4. Create a new agent (or use an existing one), then:

- Click the Settings icon next to the agent name.
  
- Go to Export and Import tab.
  
- Select Restore from ZIP, and upload the agent ZIP file.

This will import all intents, entities, and conversation flows into your agent.


Step 2: Set up ngrok

This project runs locally, so you’ll need ngrok to expose the Flask server to the internet so Dialogflow can send requests.

Download ngrok 


2. In your terminal, run:
bash
ngrok http 5000
Copy the HTTPS link that ngrok gives you (e.g., https://abc123.ngrok.io)


3
	In Dialogflow:
	•	Go to the Fulfillment tab
	•	Paste the ngrok HTTPS link into the Webhook URL field:


4. run app.py  

python app.py


now u should be able to run the Project in Localhost:8080


