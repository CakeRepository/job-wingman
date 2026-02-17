# Job Wingman - Architecture (Draft)

## High-Level Flow

1. User submits job post text/URL
2. Ingestion service normalizes content
3. Analysis agent evaluates signals:
   - compensation clarity
   - role/title consistency
   - requirement realism
   - potential scam patterns
   - remote/hybrid ambiguity
4. Scoring service computes Wingman Score + rationale
5. API returns recommendation + evidence
6. UI displays report

## Candidate Azure Stack

- Frontend: Static Web Apps
- API: Azure Functions or Container Apps
- AI: Azure OpenAI / Microsoft Foundry
- Data: Cosmos DB or Postgres
- Monitoring: Application Insights

## Agentic Pattern

- Coordinator agent orchestrates specialist evaluators
- Specialist evaluators produce structured findings
- Aggregator merges findings into final recommendation

## Trust & Safety Notes

- Explainability first (always show evidence)
- No legal advice claims
- Confidence score + uncertainty notes
- Respect privacy for pasted job content
