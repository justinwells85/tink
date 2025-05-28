# System Architecture

## Overview

The chatbot is structured into three primary layers:

1. **Frontend**: Flutter application supporting Web & Mobile.
2. **Backend**: Spring Boot REST API that connects UI, LLM, and data.
3. **LLM/Workflow Engine**: Local Ollama-hosted LLM + RAG layer for procedure lookup.

## Diagram

[Architecture diagram placeholder – consider using Mermaid.js or uploading an image]

## Key Technologies

- Ollama LLM
- Spring Boot + Maven
- AWS (for future DB, analytics, RAG)

## Future Integration

- API Gateway for OpenAI / Gemini access
- Enterprise tool integration
- Authentication/Authorization solutions
