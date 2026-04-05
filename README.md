# Exchange-Workflow_text-Voice (n8n)

This workflow automates the registration of money transfer records for an exchange service using Telegram, AI, and Google Sheets.

Users send transfer details either as text or voice through Telegram. If the message is voice, it is first transcribed into text using Google Gemini. The system then processes the content with an AI model to extract structured data such as transfer number, sender, receiver, amounts, and receiver province.

The extracted information is converted into a clean JSON format and stored in Google Sheets. If a transfer with the same number already exists, it is updated.

The workflow supports Persian input and ensures consistent data entry by enforcing a fixed structure for all records.

Requirements include n8n, Telegram Bot API, Google Gemini API, OpenAI API, and Google Sheets API.


