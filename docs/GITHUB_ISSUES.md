# Job Wingman — GitHub Issue Backlog

Use this as a copy/paste source for creating GitHub issues.

---

## Epic 1: MVP Product Foundation

### 1) Define MVP scope and acceptance criteria
- **Owner:** takescake
- **Labels:** `epic:mvp`, `type:planning`, `priority:high`
- **Description:**
  - Define what ships for hackathon MVP
  - Add explicit in/out scope
  - Add acceptance checklist tied to judging criteria
- **Done when:**
  - `docs/MVP_SCOPE.md` exists
  - Each MVP feature has testable acceptance criteria

### 2) Create project board + milestones
- **Owner:** takescake
- **Labels:** `type:ops`, `priority:high`
- **Description:**
  - Setup GitHub Project columns: Backlog / In Progress / Review / Done
  - Add milestones: Week1, Week2, Week3, Week4, Submission
- **Done when:**
  - Board populated with all issues from this file

---

## Epic 2: Scoring & Intelligence

### 3) Draft scoring taxonomy for bad-job detection
- **Owner:** Brainydaps
- **Labels:** `epic:intelligence`, `type:research`, `priority:high`
- **Description:**
  - Define signal categories (e.g., pay ambiguity, bait-and-switch, unrealistic reqs)
  - For each signal: severity, confidence hints, examples
- **Done when:**
  - `docs/SCORING_FRAMEWORK.md` created

### 4) Build labeled evaluation dataset (v1)
- **Owner:** Brainydaps
- **Labels:** `type:data`, `priority:high`
- **Description:**
  - Curate at least 50 job postings/snippets
  - Label good/investigate/skip + rationale
- **Done when:**
  - Dataset file + labeling guide committed

### 5) Implement Wingman score aggregation rules
- **Owner:** Brainydaps + Vishwadeep
- **Labels:** `type:feature`, `priority:high`
- **Description:**
  - Combine signals into 0-100 score
  - Output recommendation: Apply / Investigate / Skip
- **Done when:**
  - Unit tests for score thresholds pass

---

## Epic 3: App Engineering

### 6) Scaffold API service
- **Owner:** Vishwadeep
- **Labels:** `epic:engineering`, `type:feature`, `priority:high`
- **Description:**
  - Basic API framework setup
  - Health endpoint + structured error handling
- **Done when:**
  - Local run instructions work

### 7) Implement `POST /analyze`
- **Owner:** Vishwadeep
- **Labels:** `type:feature`, `priority:high`
- **Description:**
  - Accept pasted job text or URL
  - Return score + red flags + evidence + recommendation
- **Done when:**
  - API contract documented in README

### 8) Implement `GET /report/:id`
- **Owner:** Vishwadeep
- **Labels:** `type:feature`, `priority:medium`
- **Description:**
  - Retrieve stored analysis report
- **Done when:**
  - Works with at least one storage backend

### 9) Minimal frontend for report display
- **Owner:** Vishwadeep + Dr.Whales
- **Labels:** `type:feature`, `priority:high`
- **Description:**
  - Input box + URL field + results view
  - Clear display of rationale and evidence
- **Done when:**
  - End-to-end happy path demoable

---

## Epic 4: Azure Deployment & DevOps

### 10) Azure deployment baseline
- **Owner:** Vishwadeep
- **Labels:** `epic:azure`, `type:devops`, `priority:high`
- **Description:**
  - Deploy API + frontend to Azure
  - Set env vars/secrets safely
- **Done when:**
  - Public deployment URL available

### 11) Add monitoring and logs
- **Owner:** Vishwadeep
- **Labels:** `type:devops`, `priority:medium`
- **Description:**
  - App Insights / equivalent tracing
  - Error and latency dashboard basics
- **Done when:**
  - Team can inspect failed requests easily

### 12) CI checks + quality gates
- **Owner:** Vishwadeep
- **Labels:** `type:devops`, `priority:medium`
- **Description:**
  - Lint, test, build checks on PR
- **Done when:**
  - PRs blocked on failing checks

---

## Epic 5: UX, Demo, Submission

### 13) UX polish + explanation clarity
- **Owner:** Dr.Whales
- **Labels:** `epic:ux`, `type:design`, `priority:medium`
- **Description:**
  - Improve report readability and confidence messaging
  - Ensure outputs avoid legal-advice framing
- **Done when:**
  - Non-technical tester understands results in <30 sec

### 14) Adversarial test pass
- **Owner:** Dr.Whales + Brainydaps
- **Labels:** `type:qa`, `priority:high`
- **Description:**
  - Test weird/scammy/ambiguous listings
  - Record failure cases and fixes
- **Done when:**
  - `docs/TEST_REPORT.md` includes known limits

### 15) Architecture diagram (final)
- **Owner:** Dr.Whales
- **Labels:** `type:docs`, `priority:high`
- **Description:**
  - Diagram with Azure + agent flow + data path
- **Done when:**
  - Exported PNG/SVG in `docs/assets/`

### 16) 2-minute demo video
- **Owner:** Dr.Whales + takescake
- **Labels:** `type:submission`, `priority:high`
- **Description:**
  - Script, record, edit, upload
- **Done when:**
  - Public YouTube/Vimeo link added to README

### 17) Final submission packet
- **Owner:** takescake
- **Labels:** `type:submission`, `priority:high`
- **Description:**
  - Complete all required fields and links
  - Verify team Learn usernames included
- **Done when:**
  - Submission done at least 48h before deadline
