# RAG Bot Resume - AI Assistant

An intelligent chatbot built with n8n that answers questions about Leela Krishna Sarepalli's professional experience using Retrieval-Augmented Generation (RAG) with vector embeddings.

## Overview

This AI assistant, named "Leela", analyzes and answers questions about Leela Krishna Sarepalli's resume with high accuracy by querying a vector database containing multiple resume versions. The bot is built using n8n workflows and integrates OpenAI's GPT models with Pinecone vector storage.

## Features

- **Conversational AI Interface**: Natural language question-answering about professional experience
- **Vector-Based Retrieval**: Uses embeddings to find relevant information from stored resume documents
- **Context-Aware Responses**: Maintains conversation history with a 10-message memory buffer
- **Accurate Information Retrieval**: Clearly indicates source sections and admits when information is unavailable

## Architecture

### Workflow Components

1. **Chat Trigger**: Webhook-based public chat interface
2. **AI Agent**: Orchestrates the conversation flow with system prompts
3. **Language Model**: GPT-4.1-mini for intelligent responses
4. **Memory Buffer**: Maintains last 10 messages for context
5. **Vector Store Tool**: Retrieves relevant resume information
6. **Pinecone Database**: Stores and queries resume embeddings
7. **OpenAI Embeddings**: Converts text to vector representations

### Tech Stack

- **Workflow Automation**: n8n
- **Language Model**: OpenAI GPT-4.1-mini
- **Vector Database**: Pinecone (Index: `n8nmyresume`, Namespace: `n8nresume`)
- **Embeddings**: OpenAI Embeddings API

## About Leela Krishna Sarepalli

**Status**: Open for work in Ontario, New Brunswick, and Alberta

**Expertise**:
- Intelligent Automation
- Power Platform & Citizen Developer Advocacy
- LLM & Cloud Engineering
- Digital Transformation Consulting

### Services Offered

#### No-Code/Low-Code Development
- Agentic workflows using n8n
- Integration with Slack, HubSpot, Google Workspace, Stripe, OpenAI
- MCP server orchestration for distributed processing

**Example Solutions**:
- Lead-to-Close Sales Pipeline automation
- AI-Enhanced Customer Support Bot
- Daily Executive Summary Generator

#### Digital Transformation
- RPA tools: Microsoft Power Automate, Automation Anywhere, UiPath
- Document Intelligence & OCR Automation
- AI-Driven ChatBots & Virtual Agents

## Setup Instructions

### Prerequisites

- n8n instance (self-hosted or cloud)
- OpenAI API key
- Pinecone account and API key

### Configuration

1. **Import the Workflow**
   ```bash
   # Import the JSON file into your n8n instance
   ```

2. **Configure Credentials**
   - Add OpenAI API credentials (ID: `5GjqbfKW9YX2R414`)
   - Add Pinecone API credentials (ID: `Lv8H4EQKfsAVSpb3`)

3. **Pinecone Setup**
   - Index Name: `n8nmyresume`
   - Namespace: `n8nresume`
   - Ensure resume documents are embedded and stored

4. **Activate Workflow**
   - Enable the workflow in n8n
   - The webhook will be available at the generated URL

## Usage

### Asking Questions

The bot responds to queries about:
- Professional experience and skills
- Specific projects and accomplishments
- Technical expertise and certifications
- Availability and location preferences
- Services offered

### Response Format

Responses are structured to be:
- **Concise and precise**: Direct answers without unnecessary elaboration
- **Fact-based**: Includes specific numbers and verifiable information
- **Source-referenced**: Indicates which document section information comes from
- **Transparent**: Clearly states when information is unavailable

### Example Queries

- "What experience does Leela have with Power Automate?"
- "Where is Leela available for work?"
- "Tell me about Leela's automation projects"
- "What services does Leela offer for small businesses?"

## System Prompt

The AI assistant operates with clear guidelines:
- Specialized in analyzing Leela's resume
- Uses vector database for accurate retrieval
- States clearly when information is not available
- Provides structured, reliable insights

## Maintenance

### Updating Resume Data

To update the knowledge base:
1. Prepare new resume versions
2. Generate embeddings using OpenAI
3. Upload to Pinecone index `n8nmyresume` with namespace `n8nresume`
4. Test queries to verify new information is retrievable

### Monitoring

- Check n8n execution logs for errors
- Monitor OpenAI API usage
- Review Pinecone query performance

## License

This project is configured for personal/professional use. Modify as needed for your requirements.

## Contact

For questions about Leela Krishna Sarepalli's services or this AI assistant implementation, please reach out through the chat interface or visit the professional profiles mentioned in the resume.

---

**Note**: This is a production workflow with public webhook access. Ensure proper security measures and API rate limiting are in place.

Vist my website to chat with me

Chat here - https://www.leelakrishna.online/

<img width="404" height="604" alt="image" src="https://github.com/user-attachments/assets/54dc83d6-801f-4161-94e2-3b5882988c13" />

<img width="888" height="598" alt="image" src="https://github.com/user-attachments/assets/4612d4e9-d543-4936-8132-1854c72bb02a" />
