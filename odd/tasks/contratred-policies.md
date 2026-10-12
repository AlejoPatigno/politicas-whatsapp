# ContratRed policy adaptation

## Objective
Adapt this static legal site to describe the evidenced ContratRed platform and a WhatsApp contact channel only if enabled.

## Problem and rationale
The three HTML pages currently describe only a hypothetical automated WhatsApp channel, contain placeholders, and name providers and behaviors not evidenced in the ContratRed application. Users need a coherent platform-level privacy notice and terms without unsupported operational promises.

## Authorized scope and constraints
- Edit `index.html`, `politica-privacidad.html`, and `terminos-condiciones.html` in this clone; preserve `styles.css` and layout. Do not change the source ContratRed application, merge into main, publish a release, or open a PR. User subsequently authorized commit and push of this draft to codex/contratred-policies using the existing GitHub session.
- Use ContratRed; 12 de octubre de 2026; Manizales, Colombia; and `alejandropatinio728@gmail.com` throughout, including metadata and mail links.
- Base the text on inspected ContratRed application behavior: account and organization profiles, documents, saved resources and collaboration, public procurement sources, optional Google sign-in and AI features. WhatsApp contact is conditional, not a claimed active integration.
- Do not invent the operator's legal identity, production vendors, retention periods, payment processing, WhatsApp automation, security audits, or automated deletion. Preserve mandatory consumer and data-subject rights.
- Text-only static repo: strict TDD is configured in session, but no executable logic or test runner applies; use structural HTML checks and `git diff --check` instead.
- Delivery: `ask-on-risk`; forecast under ~400 authored changed lines (advisory only). The complete replacement exceeded that estimate because both WhatsApp-only documents required substantive correction; no text was compressed merely to meet a line count. No PR requested.

## Tasks
- [x] **T1 — Adapt the three pages.** Route: delegated direct; three non-trivial HTML edits and preparatory source reading trigger delegation. Acceptance: no template placeholders; platform-wide terms/privacy; WhatsApp only conditional; accurate data categories and optional provider/AI language; working local navigation and contact links.
- [ ] **T2 — Verify and record limits.** Route: delegated direct as part of the bounded writer task. Acceptance: `git diff --check` passes; structural checks confirm titles, language, name/date/contact, links and headings; record that operator legal identity, actual production providers, and retention rules require owner confirmation before publication.

## Evidence and progress
- Read-only source application evidence provided for `frontend/lib/registro.ts`, `frontend/components/panel-personal/ProfileForm.tsx`, `backend/store.py`, `backend/app.py`, `dashboard-backend/backend/contratred_auth.py`, `dashboard-backend/backend/api.py`, saved-resource stores, `nav_assistant.py`, and `legal_rag/answer.py` in the separate ContratRed repository.
- Baseline: branch `codex/contratred-policies` at `74386be`.
- Verification: PowerShell structural check passed for all three HTML files (one h1, Spanish language, ContratRed title and description, date, no placeholders, valid local links and mailto; both policy pages include location, contact, WhatsApp); `git diff --check` passed. Python's Windows Store launcher was unavailable, so HTMLParser was not run. No application test runner exists in this static repo.
- Changed HTML diff: 143 additions and 294 deletions, or 437 authored changed lines. This exceeds the advisory ~400-line heuristic because it replaces two unsupported WhatsApp-only documents coherently.
- Prepublication owner confirmation required: the responsible operator's legal person/entity and identification, actual production providers/deployment and enabled channels, and category-specific retention rules. Review these drafts with qualified Colombian counsel before publishing.
- Parent readback and git diff --check passed. Native assessment: medium (HTML classified executable), 464 total changed lines including this tracking file at assessment time; review_due=slice_budget_reached. Final native review remains pending; no review approval is claimed. User explicitly requested immediate commit/push of the draft despite the previously disclosed pending review. This is branch-only delivery, not a PR or legal publication.
- Next: confirm the exact registered legal name, finish prepublication facts, and complete final review before main integration or publication.
- Commit attribution: verified GitHub account AlejoPatigno (ID 111536526); use its GitHub noreply address for this command only, without changing global Git configuration.
- Runtime harness: N/A, static legal-text changes; structural checks passed.
- Rollback boundary: revert the three HTML documents together; application source and styles.css are untouched.
