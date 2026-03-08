# n8n-ai-dental-appointment-agent
AI dental appointment booking agent built with n8n, Gemini, Google Calendar, and Google Sheets

## Overview
This project automates dental appointment scheduling using an AI agent, Google Calendar, and Google Sheets.

It can:
- receive appointment requests through a webhook
- interpret patient intent with Gemini
- check appointment availability
- create calendar bookings
- log patient details for record-keeping

## Tech Stack
- n8n
- Google Gemini
- Google Calendar
- Google Sheets
- Webhooks

## Features
- AI-driven appointment handling
- Real-time calendar availability checks
- Automatic appointment creation
- Patient detail logging
- Memory for multi-turn interactions
- Extendable to voice-agent use cases

## Workflow Architecture
Webhook Trigger  
↓  
AI Agent (Gemini)  
↓  
Think Tool  
↓  
Availability Check (Google Calendar)  
↓  
Create Appointment (Google Calendar)  
↓  
Log Patient Details (Google Sheets)  
↓  
Respond to Webhook

## Example Use Case
A patient requests a dental appointment for a preferred date and time.  
The agent checks availability, suggests alternatives if needed, books the slot, and logs the patient’s insurance details and concerns.

## Files
- `workflow.json` — sanitized n8n workflow export
- `workflow.png` — workflow screenshot

## Import into n8n
1. Download `workflow.json`
2. Import it into n8n
3. Connect your own credentials for:
   - Google Gemini
   - Google Calendar
   - Google Sheets
4. Update the webhook path and calendar/sheet references

## Notes
This repository is for portfolio/demo purposes.  
All credentials, IDs, webhook values, and private references have been removed.
