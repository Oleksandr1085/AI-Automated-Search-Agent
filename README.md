# AI-Automated-Search-Agent

This project demonstrates the architecture of integrating automated workflows with Google search systems and AI-driven data processing. It has evolved from a simple search tool into an intelligent **Agentic Workflow** for business automation.

## Project Goal
The primary objective was to build an intelligent agent capable of performing targeted web searches to retrieve structured data in real-time. This data serves as a foundation for further processing and analysis by LLM models.

## Development & Implementation
1. **Infrastructure Setup:** Configured a project within the Google Cloud Platform and enabled the **Custom Search API** to allow programmatic access to search results.
2. **Search Engine Design:** Created a `Programmable Search Engine` (MySearchBot) tailored to provide clean, structured JSON responses for automated parsing.
3. **API Integration:** Implemented HTTP request nodes in **n8n**, managing authentication via `key` and `cx` (Search Engine ID) parameters to ensure secure and efficient data retrieval.
4. **Troubleshooting & Technical Analysis:** 
   - Addressed the `403 Forbidden` (Permission Denied) error through systematic API console debugging.
   - Identified and resolved limitations related to the project's verification status, specifically the requirement for linking a billing account to GCP for full API functionality.
   - Optimized **API restrictions** to maintain security and ensure requests are limited to the intended scope.
5. **Advanced Logistics Automation:** 
   - Deployed an autonomous AI Agent that functions in real-time, handling requests via Telegram.
   - Integrated Google Sheets as a knowledge base to interpret data and retrieve technical information (Custom Codes, suppliers) for inventory items.
   - Implemented `Simple Memory` for conversational context and used Google Gemini for data translation, formatting, and orchestration.

## Technical Stack
- **n8n:** AI Agentic Workflows, Orchestration, and Automation
- **LLM:** Google Gemini (data analysis, translation, and reasoning)
- **Google Workspace API:** Google Drive, Google Sheets (RAG-lite database integration)
- **Google Cloud Platform:** API and Service Management
- **Data Handling:** Persistent Memory for conversational context and JSON/Markdown formatting

## Workflow Visualization
![Workflow Schema](workflow_schema.png)
