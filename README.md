# Swahili AI Business Assistant

**Msaidizi wa Biashara kwa Kiswahili kupitia WhatsApp, unaotumia AI na n8n**

---

## Muhtasari kwa Kiswahili
Huu ni mfumo wa msaidizi wa biashara kwa wamiliki wa biashara Tanzania, unaotumia WhatsApp na AI kusaidia kusimamia bidhaa, mauzo, na gharama. Mfumo huu unatumia n8n, OpenAI, na Google Sheets kwa urahisi na ufanisi. Una msaada wa Kiswahili na umeboreshwa kwa matumizi ya kila siku ya biashara.

---

## Project Overview
Swahili AI Business Assistant is an n8n workflow that empowers Tanzanian business owners to manage their business via WhatsApp using an AI-powered assistant. The assistant supports Swahili, handles authentication, fetches business data, and provides robust error handling and logging.

## Features
- **WhatsApp AI Assistant**: Chat with your business via WhatsApp in Swahili.
- **AI-Powered**: Uses OpenAI for natural language understanding and smart responses.
- **Error Handling**: Friendly error messages for any API or system issues.
- **Logging**: All interactions and errors are logged to Google Sheets for analytics and troubleshooting.
- **Token Management**: Secure, automated login and token refresh for API access.
- **Swahili Support**: All prompts and responses are tailored for Swahili-speaking users.
- **Extensible**: Easily add more business features (e.g., add product, record sale, daily summary).

## Setup Instructions
1. **Clone the Repository**
   ```
   git clone https://github.com/Swai-D/-Swahili-AI-Business-Assistant.git
   ```
2. **Install and Run n8n**
   - [n8n Documentation](https://docs.n8n.io/)
   - Recommended: Use Docker or n8n cloud for production.
3. **Import the Workflow**
   - Open n8n UI → Import the `Swahili AI Business Assistant.json` file.
4. **Set Up Credentials**
   - WhatsApp API (Cloud API or Twilio)
   - OpenAI API Key
   - Google Sheets OAuth2 (for logging)
   - Update credential references in the workflow nodes.
5. **Prepare Google Sheet for Logging**
   - Create a sheet with columns: Timestamp, User, Query, Response, Error
   - Update the `sheetId` in the workflow.
6. **Configure WhatsApp Webhook**
   - Set up your WhatsApp webhook to point to your n8n instance.

## Usage Guide
- Business owners send messages to the WhatsApp number.
- The AI assistant responds in Swahili, fetching data on products, sales, or expenses as requested.
- If there is an error (e.g., API down, token expired), the user receives a friendly message.
- All interactions are logged for review and analytics.

## How to Extend
- Add new HTTP Request nodes for more business features (e.g., add product, record sale).
- Follow the error handling and logging pattern for each new feature.
- Update the AI Agent prompt to recognize new business intents.

## Contribution
Contributions are welcome! Please fork the repo and submit a pull request.

## License
MIT License. See LICENSE file for details.

## Contact
For support or questions, open an issue or contact [Swai-D](https://github.com/Swai-D). 