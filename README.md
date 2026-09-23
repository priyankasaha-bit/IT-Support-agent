# 🤖 IT Support AI Agent — Azure AI Foundry

## What it does
A conversational AI agent built on Microsoft Azure AI Foundry that acts as an 
IT Support assistant. It answers IT policy questions from uploaded documents 
and analyses system performance CSV data using code interpreter.

## Tools & Technologies
| Tool | Purpose |
|------|---------|
| Azure AI Foundry Portal | Created and configured the agent |
| Azure AI Projects SDK | Connected to agent via Python |
| VS Code + Foundry Toolkit | Development environment |
| File Search | Answers questions from IT policy document |
| Code Interpreter | Analyses CSV data, generates charts |
| Python 3.13 | Client application |

## How I built it
1. Created a Microsoft Foundry project on Azure portal
2. Configured agent with IT support instructions
3. Uploaded IT_Policy.txt and enabled File Search tool
4. Uploaded system_performance.csv and enabled Code Interpreter tool
5. Tested agent in Foundry playground
6. Built Python client to interact with agent programmatically

## Sample prompts
- `What's the policy for password resets?`
- `Analyse CPU usage and identify spikes above 80%`
- `Create a line chart showing memory usage trends`

## How to run it
1. Clone this repo
2. Create virtual environment:
   python -m venv labenv
   .\labenv\Scripts\Activate.ps1
3. Install dependencies:
   pip install -r requirements.txt
4. Copy .env.example to .env and add your Azure project endpoint
5. Login and run:
   az login
   python agent_with_functions.py

## Files
| File | Purpose |
|------|---------|
| agent_with_functions.py | Main Python client |
| requirements.txt | Python dependencies |
| .env.example | Environment variable template |
| IT_Policy.txt | Sample IT policy grounding document |
| system_performance.csv | Sample system metrics data |
