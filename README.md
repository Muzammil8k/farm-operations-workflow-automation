# Farm Operations Workflow Automation

An n8n-based automation system that collects farm or pond records, validates submitted data, stores valid records in Google Sheets, and sends email alerts when configured measurement thresholds are exceeded.

## Features

- Webhook-based record submission
- JavaScript validation of required fields and measurement ranges
- Conditional routing of valid and invalid submissions
- Google Sheets integration for record storage
- Email notifications for abnormal pond measurements
- Error responses for invalid submissions

## Tech Stack

- n8n
- JavaScript
- Webhooks and HTTP/REST APIs
- Google Sheets
- SMTP / Email Notifications

## Example Alert Rules

- Dissolved oxygen below 5 mg/L: trigger a low-oxygen alert.
- Temperature above 35°C: trigger a high-temperature alert.
- Invalid or missing measurements: reject the submission and return an error response.

These are demonstration thresholds, not universal aquaculture safety limits.

## Workflow

1. Receive a pond record through a webhook.
2. Validate the submitted data.
3. Route invalid records to error handling.
4. Store valid records in Google Sheets.
5. Check measurements against configured alert thresholds.
6. Send an email notification when an alert condition is met.

## Testing

The demo uses sample pond records to test valid submissions, invalid measurements, and alert conditions.

## Future Improvements

- Duplicate submission detection
- Scheduled weekly reports
- Dashboard for pond measurements
- Configurable thresholds and improved error logging

## Project Status

Demonstration project developed to practise workflow automation, API integration, and operational data processing.
