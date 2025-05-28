# Data Strategy

## RAG (Retrieval-Augmented Generation)

- Procedure documents and workflows are stored in a structured DB (AWS Aurora, DynamoDB – TBD).
- Vector embeddings indexed for retrieval during chat interaction.
- RAG layer surfaces document chunks + metadata to Ollama prompt.

## Analytics

Tracked elements:
- Workflow ID
- Timestamps per task
- Step completions
- User productivity metrics

## Escalation & Fallback

- Full searchable index of all procedures
- Manual override path
- Escalation flags tracked per workflow
