# Interview Story

## Project
Maximo AI Incident Investigator

## Why I Built It
I wanted to solve a real enterprise support problem I have seen in Maximo environments: troubleshooting production incidents requires searching through logs, documentation, XML payloads, and past knowledge articles. This increases resolution time and creates dependency on senior SMEs.

## What It Does
The application uses Retrieval-Augmented Generation to help users upload documents, ask questions, receive source-grounded answers, and generate incident summaries.

## TPM Focus
My focus was not only on building a chatbot, but on defining the product scope, success metrics, risks, architecture, roadmap, and evaluation plan.

## Technical Approach
I chose RAG because enterprise documentation changes frequently. Instead of fine-tuning a model every time documentation changes, the system can re-index updated documents and provide grounded answers with citations.

## Success Metrics
- Reduce troubleshooting time
- Improve first-contact resolution
- Increase answer trust through citations
- Measure retrieval quality using Recall@5
- Reduce hallucination risk

## Tradeoffs
- RAG is faster to update than fine-tuning, but retrieval quality depends on chunking and document quality.
- Local MVP is easier to build, but production use would require security, RBAC, audit logging, and monitoring.
- AI can assist with root cause analysis, but human review is still required before production action.

## Future Improvements
- Azure DevOps ticket creation
- Slack incident summaries
- Role-based access control
- Historical incident clustering
- Executive dashboard
