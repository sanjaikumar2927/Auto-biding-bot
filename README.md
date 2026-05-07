# Auto-biding-bot
Submitted by: Sanjaikumar
Submitted to: Califnco – AI Automation & n8n Intern
Submission Date: 07/05/2026
📌 Project Overview
The Auto Bidding Bot is an intelligent automation system that automatically detects bidding opportunities and places bids without manual intervention. It is built using free tools and designed to handle real-world constraints like rate limits, detection risk, and scalability.

🛠️ Tools & Technologies Used
Tool
Purpose
Python           -->   Core bot logic, API calls, data processing
n8n              -->   Workflow orchestration and automation triggers
Google Cloud API -->   Cloud infrastructure, authentication, and data handling
Groq API         -->   Bidding platform integration and data retrieval

🏗️ Architecture
How it works:
Trigger – n8n workflow triggers the bot on a schedule or event
Data Fetch – Python fetches available bids via Grow API
Decision Logic – Bot evaluates and selects the best bids automatically
Bid Placement – Submits bids through the API
Rate Limit Handling – Adds intelligent delays and retries to avoid detection
Logging – Results are logged via Google Cloud for monitoring

⚙️ Implementation Approach
- n8n acts as the orchestration layer, managing triggers, scheduling, and connecting services
- Python handles the core bidding logic, filtering, and API communication
- Google Cloud API is used for secure data handling and cloud-based logging
- Groq API provides the bidding data and submission endpoints
🛡️ Handling Real-World Constraints
Constraint
Solution
Rate Limits --> Randomized delays between requests, retry logic
Detection Risk --> Human-like timing patterns, rotating user agents
Scalability --> n8n workflows can run in parallel; Python scripts are modular

📁 Files Included
- bot.py – Main Python bot script
- n8n_workflow.json – Exported n8n workflow
- requirements.txt – Python dependencies
- demo/ – Demo video or screenshots
- README.md – This documentation
🚀 How to Run
Install dependencies: pip install -r requirements.txt
Set up API keys in .env file (Google Cloud, Groq API)
Import n8n_workflow.json into your n8n instance
Run manually: python bot.py or trigger via n8n
📬 Contact
Email: [sanjaikumar9792@gmail.com]
Name: Sanjaikumar
