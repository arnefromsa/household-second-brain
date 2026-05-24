# Household Second Brain Index

This vault is a household second brain for a family of five. It stores household operations, bills, maintenance, projects, people-related reference notes, documents, and long-term reference material.

This file is the root instruction document for AI assistants including Claude Code, Claude Cowork, ChatGPT Codex, and similar tools. `INDEX.md` is the source of truth. Compatibility files such as `CLAUDE.md`, `AGENTS.md`, and `CODEX.md` should point back here.

## How to Work in This Vault

- Read this file before editing.
- Preserve user-created content.
- Prefer small, clear Markdown edits.
- Do not move or rename existing files unless asked or unless a migration plan explicitly says to.
- Do not delete household records.
- Keep raw documents in `50 Documents/` or the relevant document subfolder.
- Keep active work in `10 Projects/`.
- Keep ongoing household responsibilities in `20 Areas/`.
- Put uncategorized captures in `02 Inbox/`.
- When answering a question or receiving an action update, update the most relevant durable note if it creates, corrects, clarifies, completes, or changes household knowledge.
- Log important questions, unresolved gaps, and follow-up actions in `02 Inbox/Question Log.md`.
- After a major knowledgebase update, refresh the household dashboard or record why it was not needed.
- Use dates in `YYYY-MM-DD` format.
- Ask before adding sensitive personal, medical, financial, or identity information.

## Folder Rules

- `02 Inbox/`: temporary capture and processing.
- `10 Projects/`: active efforts with a finish line.
- `20 Areas/`: ongoing responsibilities.
- `30 People/`: practical notes about household members.
- `40 Resources/`: stable reference material.
- `50 Documents/`: raw files, bills, statements, receipts, policies, scans, and manuals.
- `60 Dashboards/`: generated or hand-built dashboard views, including `Household Dashboard.html` and the instructions for maintaining it.
- `90 Archive/`: inactive or superseded material.

## Dashboard Rules

The household dashboard is a readable HTML control panel for the household. It should live at:

`60 Dashboards/Household Dashboard.html`

Build and maintenance instructions live at:

`60 Dashboards/Household Dashboard Instructions.md`

When building or updating the dashboard:

- Treat Markdown notes as the source of truth.
- Do not invent household data just to fill the interface.
- Prefer a static, self-contained HTML file with embedded CSS and minimal JavaScript.
- Do not require a web server unless the user explicitly asks for live data loading.
- Show source links back to the notes that supplied each dashboard section.
- Make the dashboard useful at a glance: priorities, bills, maintenance, family logistics, emergency information, recent changes, and open questions.
- If the dashboard exposes sensitive information, ask before adding it.
- When the dashboard reveals stale or missing information, update the relevant note and record meaningful gaps in `02 Inbox/Question Log.md`.

## Major Update Dashboard Refresh

A major knowledgebase update is any change that materially affects the household picture. Examples:

- Importing or reorganizing household records.
- Adding or changing active projects.
- Adding, changing, or resolving bills, subscriptions, insurance, or renewals.
- Adding or changing maintenance tasks, contractors, rooms, or household systems.
- Updating emergency, school, health, vehicle, routine, or people-related information.
- Processing several inbox items at once.
- Making broad structural changes to the vault.

After a major update:

1. Update the relevant Markdown notes first.
2. Check whether `60 Dashboards/Household Dashboard.html` needs to change.
3. If it exists, refresh it so it reflects the updated notes.
4. If it does not exist yet, update `60 Dashboards/Household Dashboard Instructions.md` only if the requested dashboard behavior has changed.
5. Add a short entry to `02 Inbox/Question Log.md` if the update revealed a meaningful gap or follow-up action.

If the assistant supports delegated work or subagents, it should spin off a dashboard-refresh subagent after major updates. The subagent should read `INDEX.md`, read `60 Dashboards/Household Dashboard Instructions.md`, inspect the changed notes, update the dashboard, and report back with files changed and any gaps found.

If subagents are not supported, the active assistant should perform the dashboard refresh itself before finishing the task.

## Naming

Use clear filenames. For dated records, use:

`YYYY-MM-DD - Provider - Description.ext`

Examples:

- `2026-05-12 - Energy Provider - Electricity Bill.pdf`
- `2026-04-03 - Plumber Name - Kitchen Sink Invoice.pdf`
- `2026-01-15 - Insurance Provider - Home Insurance Renewal.pdf`

## Linking

Use Markdown links between related notes. Prefer linking to duplicating the same information in multiple places.

## Sensitive Information

Be careful with medical, financial, identity, account, password, and child-related information. Do not add unnecessary sensitive details. Never invent personal details.

## Self-Learning Loop

When a household member asks a question or provides an action update, treat it as a maintenance signal for the vault. Action updates include decisions made, tasks completed, bills paid, appointments booked, maintenance performed, documents added, providers changed, or priorities updated.

1. Read the relevant notes.
2. Answer from existing vault content when possible, or acknowledge the action update.
3. If information is missing, say what is missing.
4. If the user provides new facts or reports progress, update the relevant durable note.
5. If old information is wrong or outdated, correct the relevant note.
6. If an action changes priorities, due dates, status, ownership, bills, maintenance, documents, or projects, update those notes too.
7. Add a short entry to `02 Inbox/Question Log.md` when the exchange revealed a gap, caused an update, or created a follow-up action.
8. Add action items to `01 Current Priorities.md` or the relevant project note when needed.

The log is for traceability. It is not the main knowledge base.
