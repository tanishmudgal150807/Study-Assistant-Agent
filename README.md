# Study-Assistant-Agent

An AI-powered Study Assistant Agent that creates personalized daily study plans and automatically reschedules them when the user's available study time changes.

## Features

- Generates daily study plans
- Considers available study time
- Prioritizes subjects
- Includes study sessions and breaks
- Remembers the current study plan
- Automatically reschedules when available time changes

## Technologies Used

- n8n
- Google Gemini
- AI Agent
- Simple Memory

## How It Works

The user enters their subjects and available study time through the n8n chat interface.

The AI Agent creates a personalized study plan using Google Gemini.

Simple Memory allows the agent to remember the current study plan and modify it when the user has less available time.

### Example

User:

"I need to study DSA, Java and Maths. I have 4 hours today."

The agent generates a 4-hour study plan.

User:

"I only have 1 hour today. Reschedule my plan."

The agent remembers the subjects and creates a new 1-hour plan.

## Workflow

Chat Trigger → AI Agent → Gemini

Simple Memory is connected to the AI Agent.

## How to Run

1. Open n8n.
2. Import `study-assistant-agent.json`.
3. Add your own Google Gemini API credential.
4. Open the Chat Trigger.
5. Start chatting with the Study Assistant Agent.

## Sample Inputs

- I need to study DSA, Java and Maths. I have 4 hours today.
- I only have 2 hours today. Reschedule my plan.
- I have an exam tomorrow. Prioritize DSA.
