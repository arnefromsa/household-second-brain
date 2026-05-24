# Prompt: Build the Household Second Brain

Use this prompt with Claude Code, Claude Cowork, ChatGPT Codex, or another file-editing AI assistant to create the recommended household second brain structure.

## Prompt

You are working inside a Markdown vault used as a household second brain for a family of five. Build the structure described below.

The vault must be useful as a household operating manual and must remain readable as plain files. Do not assume a single app or AI tool. The vault may be opened by Claude Code, Claude Cowork, ChatGPT Codex, Obsidian, or a normal file browser.

Before making changes:

- Inspect the existing root folder.
- Preserve all existing user-created files.
- Do not delete, overwrite, or rename existing files unless explicitly instructed.
- If a target file already exists, update it carefully instead of replacing it blindly.
- Keep edits in Markdown unless a folder or raw document location is required.

Create this top-level structure:

```text
Second Brain/
  INDEX.md
  CLAUDE.md
  AGENTS.md
  CODEX.md
  00 Home.md
  01 Current Priorities.md
  02 Inbox/
  10 Projects/
  20 Areas/
  30 People/
  40 Resources/
  50 Documents/
  90 Archive/
```

`INDEX.md` is the canonical root instruction file. `CLAUDE.md`, `AGENTS.md`, and `CODEX.md` are compatibility files for different assistants. They should point to `INDEX.md` and briefly state that `INDEX.md` is the source of truth.

Create these dashboard notes:

```text
02 Inbox/Inbox.md
02 Inbox/Question Log.md
02 Inbox/To Process.md
10 Projects/Projects.md
20 Areas/Areas.md
20 Areas/Household/Household.md
20 Areas/Household/Utilities/Utilities.md
20 Areas/Household/Utilities/Electricity/Electricity.md
20 Areas/Household/Utilities/Electricity/Usage.md
20 Areas/Household/Utilities/Electricity/Bills.md
20 Areas/Household/Utilities/Internet/Internet.md
20 Areas/Household/Utilities/Water/Water.md
20 Areas/Household/Utilities/Gas/Gas.md
20 Areas/Household/Maintenance/Maintenance.md
20 Areas/Household/Maintenance/Maintenance Log.md
20 Areas/Household/Maintenance/Contractors.md
20 Areas/Household/Maintenance/Rooms/Kitchen.md
20 Areas/Household/Maintenance/Rooms/Bathrooms.md
20 Areas/Household/Maintenance/Rooms/Bedrooms.md
20 Areas/Household/Maintenance/Rooms/Garage.md
20 Areas/Household/Maintenance/Rooms/Yard.md
20 Areas/Household/Finance/Household Finance.md
20 Areas/Household/Finance/Bills.md
20 Areas/Household/Finance/Budget.md
20 Areas/Household/Finance/Subscriptions.md
20 Areas/Household/Finance/Insurance.md
20 Areas/Household/Vehicles/Vehicles.md
20 Areas/Household/Health/Health.md
20 Areas/Household/School/School.md
20 Areas/Household/Food/Meal Planning.md
20 Areas/Household/Food/Recipes.md
20 Areas/Household/Food/Shopping List.md
20 Areas/Household/Routines/Routines.md
20 Areas/Household/Routines/Cleaning.md
20 Areas/Household/Routines/Chores.md
20 Areas/Household/Routines/Waste and Recycling.md
20 Areas/Household/Emergency/Emergency.md
20 Areas/Household/Emergency/Contacts.md
20 Areas/Household/Emergency/Shutoffs.md
30 People/People.md
40 Resources/Resources.md
50 Documents/Documents.md
90 Archive/Archive.md
```

Create these raw-file folders:

```text
20 Areas/Household/Utilities/Electricity/Bills/
20 Areas/Household/Utilities/Electricity/Usage/
50 Documents/10 Property/
50 Documents/20 Utilities/Electricity/
50 Documents/20 Utilities/Internet/
50 Documents/20 Utilities/Water/
50 Documents/30 Finance/Tax/
50 Documents/30 Finance/Bank/
50 Documents/30 Finance/Insurance/
50 Documents/40 Medical/
50 Documents/50 School/
50 Documents/60 Vehicles/
50 Documents/70 Warranties and Manuals/
50 Documents/80 Receipts/
90 Archive/Projects/
90 Archive/Old Providers/
90 Archive/Old Documents/
```

Write `INDEX.md` with these instructions:

```markdown
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
- Use dates in `YYYY-MM-DD` format.
- Ask before adding sensitive personal, medical, financial, or identity information.

## Folder Rules

- `02 Inbox/`: temporary capture and processing.
- `10 Projects/`: active efforts with a finish line.
- `20 Areas/`: ongoing responsibilities.
- `30 People/`: practical notes about household members.
- `40 Resources/`: stable reference material.
- `50 Documents/`: raw files, bills, statements, receipts, policies, scans, and manuals.
- `90 Archive/`: inactive or superseded material.

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
```

Write each compatibility file as:

```markdown
# Assistant Instructions

This vault uses `INDEX.md` as the source of truth for assistant instructions.

Before making changes, read `INDEX.md`.
```

Write `00 Home.md` with:

```markdown
# Home

## Household Snapshot

## Current Priorities

- [[01 Current Priorities]]
- [[02 Inbox/Question Log]]

## Key Dashboards

- [[10 Projects/Projects]]
- [[20 Areas/Areas]]
- [[20 Areas/Household/Household]]
- [[20 Areas/Household/Utilities/Utilities]]
- [[20 Areas/Household/Maintenance/Maintenance]]
- [[20 Areas/Household/Finance/Bills]]
- [[20 Areas/Household/Emergency/Emergency]]
- [[30 People/People]]
- [[50 Documents/Documents]]

## Active Projects

## Upcoming Deadlines

## Emergency Links

- [[20 Areas/Household/Emergency/Emergency]]
- [[20 Areas/Household/Emergency/Contacts]]
- [[20 Areas/Household/Emergency/Shutoffs]]

## Recently Updated
```

Write `01 Current Priorities.md` with:

```markdown
# Current Priorities

## This Week

## This Month

## Waiting On

## Bills and Money

## House and Maintenance

## Family Logistics

## Parking Lot
```

Write `02 Inbox/Question Log.md` with:

```markdown
# Question Log

Use this as a lightweight ledger of questions that improved the vault. Do not use it as the main knowledge base. Durable information should be moved into the relevant project, area, person, resource, or document note.

## Template

### YYYY-MM-DD

#### Question

#### Answered From

#### Updated Notes

#### Follow-up
```

Use these templates when creating project, service provider, maintenance, and decision notes.

Project template:

```markdown
# Project Name

Status:
Owner:
Started:
Target date:
Related area:

## Outcome

## Next Actions

## Decisions

## Notes

## Related Files
```

Service provider template:

```markdown
# Provider or Service Name

Status:
Account number:
Login:
Renewal date:
Billing cycle:
Payment method:

## Summary

## Current Plan

## Important Dates

## Support

## Related Documents

## Notes
```

Maintenance template:

```markdown
# Maintenance Item

Status:
Owner:
Location:
Priority:
Next action:
Due date:

## Problem

## History

## Quotes

## Decision

## Related Files
```

Decision template:

```markdown
# Decision: Title

Date:
Status:
People involved:

## Context

## Options

## Decision

## Reasoning

## Follow-up
```

For all other dashboard notes, create concise headings appropriate to the file name. Include links to child notes where helpful. Avoid overfilling empty notes with invented household details.

Existing content and imports:

- The old `House/` folder has been moved out while this vault is still being designed.
- Treat this as a blueprint build first.
- Do not assume old household files are currently present in the vault.
- Create the new structure without importing legacy files.
- If a `House/` folder is later reintroduced, leave it untouched unless explicitly asked to migrate it.
- Do not move bills, PDFs, CSVs, or existing provider notes unless explicitly asked.

After creating the structure:

- Report which files and folders were created.
- Report any existing files that were left untouched.
- Mention any conflicts or files that already existed.
