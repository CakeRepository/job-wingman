# Job Wingman

AI assistant for job applicants to quickly detect misleading, low-quality, or scam-like job listings before they waste time applying.

## Hackathon Context

This project is being built for the **AI Dev Days Hackathon**.

It is designed to satisfy the core requirements:
- **AI technology:** planned use of Microsoft Agent Framework + Azure AI services
- **Azure deployment:** deployable to Azure (Container Apps / Functions)
- **GitHub development:** public repo, VS Code workflow, Copilot-assisted development

## Problem

Job seekers lose time and energy on listings that are vague, deceptive, or not aligned with the actual role.

## Solution

Job Wingman analyzes a job posting and returns:
- **Wingman Score (0-100)** for listing quality/trustworthiness
- **Red flags** (e.g., unrealistic requirements, compensation ambiguity, bait-and-switch indicators)
- **Evidence snippets** from the posting
- **Recommendation**: Apply / Investigate / Skip

## Planned Features (MVP)

- Paste job description text or URL
- Multi-signal analysis agent
- Risk categories + confidence scores
- Explanation-first output (transparent reasons)
- Save/share report

## Project Structure

- `src/` — app and agent code
- `infra/` — deployment IaC and Azure config
- `docs/` — architecture, hackathon checklist, pitch assets
- `tests/` — automated tests

## Quick Start

```bash
# 1) install deps (when package.json is added)
# npm install

# 2) run app locally
# npm run dev
```

## Hackathon Submission Checklist

See `docs/HACKATHON_CHECKLIST.md`.

## Next Steps

1. Build intake flow (text/URL)
2. Implement scoring heuristics + LLM reasoning pass
3. Add Azure deploy target
4. Add demo script + 2-minute video outline
5. Publish public GitHub repo
