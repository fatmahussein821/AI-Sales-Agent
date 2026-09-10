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
  


