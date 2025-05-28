# Environment Topology

## Local Development

```
[Flutter UI] ⇄ [Spring Boot API] ⇄ [Local RAG DB] ⇄ [Ollama LLM]
```

## Planned Deployment (Staging/Production)

```
[Browser/Mobile App]
        ⇅
[API Gateway] — Auth & Rate Limit
        ⇅
[Spring Boot App]
        ⇅         ⇅         ⇅
  [MCP Tools]  [Vector DB]  [LLM API]
```

## Services

- LLM: Ollama for local, Gemini/OpenAI via internal gateway later
- RAG DB: AWS-hosted (Aurora or DynamoDB + vector engine)
- Orchestration layer within Spring Boot
- Optional tools API via MCP

