# Arogya Mitra Tele‑Agent
Arogya Mitra is an AI-powered healthcare platform connecting patients and doctors.
arogya_mitra_teleagent is the voice-based gateway for patients who do not own a
smartphone. Patients can dial a local number from any basic keypad phone and interact with
an AI agent powered by Vapi, with all workflows handled seamlessly via Make.com (formerly
Integromat)—no custom server is required.

# Key Features
1 Phone‑first access – Works on any keypad/feature phone - no smartphone or app required
2 Conversational AI – Voice-based interaction in local languages powered by Vapi agents
3 No server needed – All backend workflows handled through Make.com scenarios
4 Data integration – All call data (summary, user info, symptoms) stored in a connected database
(Firestore)

#  How It Works
<img width="1215" height="1476" alt="Flowcharts" src="https://github.com/user-attachments/assets/ba32b765-5e9d-4cd1-a7b4-3486f95ba466" />


#  Creating the Agent on Vapi – Step by Step
1. Open the Dashboard
2. Go to Assistant -> click on create Assitant.
3. Select the model and message.
4. Type the System Prompt.
5. Select Voice provider and voice as per location.
6. Go to Analysis Section and give the prompt for Summary so as to get the conversational summary.

Assistant is ready!
Calling-
1. Go to Phone Number
2. Immport Twilio Number , SOD , Auth Token and label
3. Select the inbound and outbound call options.
4. Go to make.com
5. Create a Scenario and then select the webhook , copy url
6. In vapi select the advance tab and in messaging paste the url for the webhook integration.
7. Now in make create a connection from webhook to a another node of firestore
8. Add the client ID and Secret key obtained from google console outh2.0 for storing the summary to the firestore
9. Add the relevant details how do you want the summary to be stored.
10. Start the webhook.
    
# LICENCE
 This project is licensed under the MIT License – see 
LICENSE for detail

# 🙏 Acknowledgements
Vapi – for their no-code voice AI platform
Make.com – for their workflow automation engine
OpenAI GPT-4o – voice intelligence
“Bridging the healthcare divide for all—no smartphone required.” — Arogya Mitra Tea

