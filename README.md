# Household Second Brain

A Markdown-first household knowledge base for managing the practical life of a home: bills, maintenance, documents, projects, routines, family logistics, and long-term reference notes.

It is designed to work as plain files, in Obsidian, or with AI coding assistants such as Claude Code, Claude Cowork, ChatGPT Codex, and similar tools.

## What This Is

This project is a starter structure for a household "second brain". It gives you a ready-made folder system, dashboard notes, assistant instructions, and conventions for keeping a home organized over time.

The goal is not to create a perfect personal productivity system. The goal is to make household information easy to find, update, and hand off.

It is inspired in part by Andrej Karpathy's idea of a simple Markdown-based, LLM-friendly second brain: a folder of plain text notes that humans can maintain and AI assistants can read, update, and reason over.

Reference: [Karpathy second brain gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)

## Features

- Plain Markdown notes that work anywhere.
- Root assistant instructions in `INDEX.md`.
- Compatibility files for AI tools: `CLAUDE.md`, `AGENTS.md`, and `CODEX.md`.
- Household areas for utilities, finance, maintenance, emergency info, food, routines, health, school, vehicles, and people.
- Project tracking for active household work.
- Document folders for bills, receipts, policies, manuals, and records.
- A self-learning loop: questions and action updates can update the knowledge base instead of disappearing into chat history.
- Dashboard instructions for building a local `Household Dashboard.html`.
- Blueprint and research notes kept in `999 Blueprint/`.

## Why Use It

- Keeps household information out of scattered chats, emails, and memory.
- Makes recurring tasks and bills easier to track.
- Gives AI assistants clear rules for safely editing the vault.
- Separates active projects, ongoing responsibilities, documents, and archives.
- Stays portable because the core format is just folders and Markdown.

## Structure

```text
.
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
  60 Dashboards/
  90 Archive/
  999 Blueprint/
```

## How It Works

Start at `00 Home.md` for navigation and `01 Current Priorities.md` for what matters now.

Use:

- `02 Inbox/` for quick capture and unprocessed notes.
- `10 Projects/` for active work with a finish line.
- `20 Areas/` for ongoing household responsibilities.
- `30 People/` for practical household-member notes.
- `40 Resources/` for stable reference material.
- `50 Documents/` for raw files and important records.
- `60 Dashboards/` for generated or hand-built dashboard views.
- `90 Archive/` for inactive or superseded material.

## AI Assistant Support

AI assistants should read `INDEX.md` before making changes. It explains how to file information, preserve user content, handle sensitive data, update dashboards, and use the self-learning loop.

The compatibility files are intentionally small:

- `CLAUDE.md`
- `AGENTS.md`
- `CODEX.md`

Each points back to `INDEX.md` as the source of truth.

## Self-Learning Loop

When someone asks a useful household question or reports an action update, the exchange should improve the vault.

For example:

1. Answer from existing notes where possible.
2. If information is missing, say what is missing.
3. If new facts or progress updates are provided, update the relevant durable note.
4. If the update changes a task, bill, project, maintenance item, document, or priority, update that item too.
5. If the exchange revealed a gap or follow-up action, log it in `02 Inbox/Question Log.md`.

The log is an audit trail, not the main knowledge base.

## Dashboard

`60 Dashboards/Household Dashboard Instructions.md` describes how to build a local `Household Dashboard.html`.

The dashboard is intended to show:

- Current priorities
- Attention queue
- Bills and renewals
- Maintenance radar
- Family logistics
- Active projects
- Emergency links
- Recent learning
- Documents to file

After major knowledge base updates, assistants should check whether the dashboard needs refreshing.

## Getting Started

1. Clone or copy this repository.
2. Open the folder in your Markdown editor, Obsidian, Claude Code, ChatGPT Codex, or another file-aware assistant.
3. Read `INDEX.md`.
4. If you are starting from the blueprint, prompt your LLM or file-aware assistant to execute the instructions in `999 Blueprint/household-second-brain-prompt.md`.
5. Open `00 Home.md`.
6. Add your current priorities to `01 Current Priorities.md`.
7. Capture loose information in `02 Inbox/Inbox.md`.
8. Add household details gradually under `20 Areas/Household/`.
9. Store bills, receipts, manuals, and policies under `50 Documents/`.

Start small. A useful household second brain grows from repeated updates, not from filling every file on day one.

## Loading Your Content With Inbox

Use `02 Inbox/` as the safe landing zone for existing household information.

Good inbox candidates:

- Bills, receipts, statements, policies, manuals, and CSV exports.
- Notes copied from chats, emails, documents, or old systems.
- Photos or scans that need filing.
- Rough lists of providers, projects, maintenance tasks, routines, or priorities.

Suggested workflow:

1. Drop files or rough notes into `02 Inbox/`.
2. Add context in `02 Inbox/Inbox.md` or `02 Inbox/To Process.md`.
3. Ask your LLM or file-aware assistant to process the inbox.
4. The assistant should move durable information into the relevant notes and folders.
5. The assistant should leave raw records in `50 Documents/` or the appropriate document folder.
6. If processing reveals missing information or follow-up actions, log them in `02 Inbox/Question Log.md`.
7. Keep the inbox temporary. Once something has a proper home, remove it from the processing list.

This keeps imports low-risk: you can capture first, then organize deliberately.

## Extending It

You can extend the structure by adding:

- New household areas, such as pets, garden, rentals, or travel.
- Templates for providers, maintenance items, decisions, and projects.
- Scripts that generate dashboards from Markdown.
- More dashboard pages, such as finance, maintenance, or document dashboards.
- Sync or backup workflows.
- Private encrypted storage for sensitive records.

Keep extensions boring and obvious. If a future household member or assistant cannot guess where something belongs, the structure is too clever.

