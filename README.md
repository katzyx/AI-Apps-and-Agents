# AI-Apps-and-Agents
Prototype Universal HelpDesk Agent on Flowise

The agent intelligently routes questions to the correct knowledge base (HR or IT) and escalate to a human agent if the query cannot be resolved.

## Requirements
- Docker Desktop

## Run Flowise
docker run -d --name flowise -p 3000:3000 -v ./data:/root/.flowise flowiseai/flowise:latest

## Open UI
http://localhost:3000

## Import Agentflows
1. Go to Agentflows
2. Import `Helpdesk Agent Agents.json`

## Configure Credentials
- Add Google GenAI / Gemini API key
- Add Pinecone API key + index + namespace config (hr/it)

## Demo Queries
- "Who is eligible for wfh?"
- "How do I reset my password?"
- "What is the parental leave policy?"
