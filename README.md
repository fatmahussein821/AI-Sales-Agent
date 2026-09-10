# AI Sales Agent

An **n8n sales-outreach automation workflow** that captures structured leads, researches company context, generates personalized HTML email drafts with Gemini, and routes them through human approval before Gmail delivery.

## What it does

- Receives or processes structured lead information.
- Stores lead records in Google Sheets.
- Fetches relevant company information for personalization.
- Uses Google Gemini to generate concise, context-aware outreach copy.
- Builds an HTML email draft with lead-specific details.
- Includes a human approval step before sending through Gmail.

## Workflow design

`Lead intake → Data validation → Google Sheets → Company research → Gemini personalization → HTML email draft → Human approval → Gmail`

## Integrations

- n8n
- Google Sheets
- Google Gemini
- Gmail
- HTTP requests and JavaScript transformations

## Repository contents

- `Ai sales agent.json` — exported n8n workflow.
- `README.md` — workflow overview and setup notes.

## Setup

1. Import `Ai sales agent.json` into n8n.
2. Configure the Google Sheets, Gemini, and Gmail credentials.
3. Select the destination spreadsheet and map the expected lead columns.
4. Review the prompt and email template for the target audience.
5. Test the workflow with sample leads.
6. Keep the approval step enabled before activating production sending.

The exported workflow is intended as a reusable template and should be reviewed for credential, spreadsheet, and email-policy requirements before activation.

## Safety note

This workflow is designed to keep a person in the loop before outbound communication. Do not place API keys, OAuth tokens, private contact data, or production credentials in the repository.
