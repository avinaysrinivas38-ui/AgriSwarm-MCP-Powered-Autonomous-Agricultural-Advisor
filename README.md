# AgriSwarm-MCP-Powered-Autonomous-Agricultural-Advisor
AgriSwarm is an autonomous, MCP-powered multi-agent system designed for agricultural resilience. It continuously monitors live environmental and soil data. When anomalies like frost or drought are detected, specialized AI agents instantly collaborate to formulate and dispatch actionable, localized agronomic alerts directly to farmers via SMS.
# 🌾 AgriSwarm: MCP-Powered Autonomous Agricultural Advisor

AgriSwarm is a multi-agent system designed to monitor agricultural data and autonomously dispatch localized interventions to farmers. Built for Hackathon 2026.

## Architecture
- **Data Scraper:** Pulls mock IoT sensor data and API weather forecasts.
- **Agronomy Engine:** RAG-powered agent that analyzes anomalies against agricultural research.
- **Localization:** Translates and formats technical data into SMS/WhatsApp alerts.
- **Supervisor:** Audits the workflow and manages tool failures.

## Quick Start
1. Clone the repo.
2. Install dependencies: `pip install -r requirements.txt`
3. Copy `.env.example` to `.env` and add your API keys (Twilio, OpenAI/Anthropic).
4. Run the orchestration: `python src/main.py`
5. Open `dashboard/index.html` in your browser to view the live agent reasoning loop.

## Technologies Used
* LangGraph / CrewAI
* Model Context Protocol (MCP)
* Twilio API
* Supabase
