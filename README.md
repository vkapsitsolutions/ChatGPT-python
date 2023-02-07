# ChatGPT-python

# OpenAI Whatsapp Bot using Twilio

# Installation
Open terminal
Create virtual environment in working directory and activate it.

git clone https://github.com/Jayesh00001/04_OpenAI_Twilio_Whatsapp_Bot

$ pip install -r reqt.txt

# Requirements
python>=3.8, if you don't have download from https://www.python.org/

OpenAI API Key from https://platform.openai.com/account/api-keys 

# Setup
Need to setup the OpenAI API as .env file, copy and paste below code. Add it to your working directory where your app "app.py" is running. 
Also download and put the ngrok.exe file in working directory.

export OPENAI_API_KEY=[YOUR OPENAI API ACCESS KEY]

export TWILLIO_AUTH_TOKEN=[TWILLIO_AUTH_TOKEN]

export TWILLIO_ACCOUNT_SID=[TWILLIO_ACCOUNT_SID]

export FROM_WHATSAPP_NUMBER=[FROM_WHATSAPP_NUMBER]  # +14155238886

export MAX_TOKENS=[NUMBER OF MAX TOKENS IN EACH REPLY]

export CONVERSATION_EXPIRES_MINS=[N MINUTES UNTIL A CONVERSATION IS ERASED FROM MEMORY]

export ALLOWED_PHONE_NUMBERS=[+1234567890, +1987654321]

# Installation ngrok
1. Download and install ngrok from "https://ngrok.com/download"
2. Open another terminal 
3. Run "ngrok http 5000". The ngrok terminal shows the Forwording URL starting with "https:// " copy it
& return to Twilio Console Whatsapp messages sandbox [WHEN A MESSAGE COMES IN] field and append the "/bot", since that is our endpoint.

The URL from ngrok is "https://ad7e4814affe.ngrok.io/bot" but yours will be different.

# To run the Whatsapp bot
Open another terminal and run the app with command "python app.py".

# Configure Twilio WhatsApp
Use your smartphone to send a WhatsApp message of the phrase to your assigned WhatsApp number. 
If you are successful, you should receive a message as

"""Twilio Sandbox: ✅ You are all set! The sandbox can now send/receive messages from whatsapp:+14155238886. Reply stop to leave the sandbox any time"""

# Chatbot
After following the instructions in the Twilio Sandbox for Whatsapp Tutorial you should be able to join your sandbox and start chatting with the bot inmediately. 
 
<img width="625" alt="Capture" src="https://user-images.githubusercontent.com/104774003/207853041-3b636da0-065d-43ed-92c8-6eb124046734.PNG">
