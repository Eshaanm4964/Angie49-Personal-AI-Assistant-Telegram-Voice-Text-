**🚀 Overview**

Angie49 is a powerful personal AI assistant that operates directly inside Telegram, supporting both voice and text interactions.

Angie helps you manage daily productivity tasks such as:

📩 Email summarization

📅 Calendar lookup

✅ Task reminders

📇 Contact retrieval

🎙️ Voice message transcription

It integrates OpenAI, Telegram Bot API, Gmail API, Google Calendar, and Baserow into a seamless intelligent workflow.

🧠 How Angie Works
🔹 1. Telegram Trigger

The workflow begins when a user sends a message to the Telegram bot.

The system:

Detects whether the message is text or voice

Routes it accordingly

🔹 2. Voice Handling (If Voice Message)

If the message is a voice note:

The voice file is retrieved from Telegram

It is sent to OpenAI Speech-to-Text API

The audio is transcribed into text

The text is forwarded to the AI assistant

This enables completely hands-free interaction.

🔹 3. AI Assistant (Angie)

The transcribed or typed text is passed to Angie, the AI brain of the system.

Angie:

Understands user intent

Decides which tool(s) to call

Gathers required data

Generates a contextual response

🔹 4. Tools Integration

Angie is equipped with specialized tools:

📩 Get Email

Uses Gmail API

Fetches recent emails

Filters by date

Summarizes key points

📅 Get Calendar

Connects to Google Calendar API

Retrieves events for specific dates

Supports daily or range-based queries

✅ Get Tasks

Connects to Baserow

Fetches to-do list entries

Filters by status or due date

📇 Get Contacts

Uses Baserow database

Retrieves saved contact details

🔹 5. Response Generation

After gathering information:

Angie composes a natural-language response

Sends the reply back to the user via Telegram

Maintains conversational context

🏗️ System Architecture
Telegram User
        ↓
Telegram Trigger
        ↓
Voice or Text Detection
        ↓
(OpenAI Speech-to-Text if Voice)
        ↓
AI Assistant (Angie)
        ↓
Tool Selection & Execution
        ↓
Response Generation
        ↓
Telegram Reply

🧩 Tech Stack

Telegram Bot API

OpenAI API (GPT + Speech-to-Text)

Gmail API

Google Calendar API

Baserow (Open-source Airtable alternative)

Workflow Automation (e.g., n8n)

📦 Project Structure
angie49/
│
├── telegram-trigger/
├── voice-handler/
├── ai-assistant/
├── tools/
│   ├── get-email/
│   ├── get-calendar/
│   ├── get-tasks/
│   └── get-contacts/
│
├── response-handler/
└── README.md

🔐 Required API Credentials

To run Angie, you need:

Telegram Bot Token

OpenAI API Key

Gmail API Credentials

Google Calendar API Credentials

Baserow API Token

⚙️ Setup Instructions
1️⃣ Create Telegram Bot

Open Telegram

Search for @BotFather

Create a new bot

Copy the Bot Token

2️⃣ Configure APIs

Enable Gmail API

Enable Google Calendar API

Generate OAuth credentials

Obtain OpenAI API key

Create Baserow tables:

Tasks

Contacts

3️⃣ Configure Workflow

Import workflow into automation platform (e.g., n8n)

Add credentials

Activate workflow

Test using Telegram

💬 Example Commands
Summarize today's emails
Do I have meetings tomorrow?
What tasks are due this week?
Get contact details for Rahul


🎙️ Voice messages work exactly the same.

🎯 Use Cases

Personal productivity assistant

Executive assistant bot

Daily email digest automation

Smart task management

Voice-controlled AI companion

🔮 Future Improvements

Smart email prioritization

Auto reminders for urgent tasks

Meeting summaries

WhatsApp integration

Personalized memory layer

Multi-user support
