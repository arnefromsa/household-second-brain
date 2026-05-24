# Household Dashboard Instructions

Build `Household Dashboard.html` as a local, static household control panel. The dashboard should be useful even when opened directly from the filesystem, so prefer one self-contained HTML file with embedded CSS and minimal JavaScript.

Target path:

```text
60 Dashboards/Household Dashboard.html
```

## Purpose

The dashboard is the household cockpit: a calm, scannable view of what matters now. It should help someone answer:

- What needs attention today or this week?
- Which bills, renewals, and maintenance tasks are coming up?
- What projects are active?
- What family logistics are unresolved?
- Where are the emergency notes?
- What did the second brain recently learn?

## Source Notes

Use these notes as the first sources:

- `00 Home.md`
- `01 Current Priorities.md`
- `02 Inbox/Question Log.md`
- `10 Projects/Projects.md`
- `20 Areas/Household/Household.md`
- `20 Areas/Household/Finance/Bills.md`
- `20 Areas/Household/Finance/Subscriptions.md`
- `20 Areas/Household/Maintenance/Maintenance.md`
- `20 Areas/Household/Maintenance/Maintenance Log.md`
- `20 Areas/Household/Routines/Routines.md`
- `20 Areas/Household/Food/Meal Planning.md`
- `20 Areas/Household/Emergency/Emergency.md`
- `20 Areas/Household/Emergency/Contacts.md`
- `20 Areas/Household/Emergency/Shutoffs.md`
- `30 People/People.md`
- `50 Documents/Documents.md`

## Suggested Layout

Create a single-page dashboard with these sections.

### Household Pulse

A compact top strip showing:

- Today date
- Current week focus
- Number of active projects
- Number of waiting items
- Upcoming bills count
- Maintenance items needing attention

### This Week

Pull from `01 Current Priorities.md`.

Show:

- This week
- Waiting on
- Bills and money
- House and maintenance
- Family logistics

### Attention Queue

A prominent list of items that need a decision, action, or follow-up.

Sources:

- `01 Current Priorities.md`
- `02 Inbox/To Process.md`
- `02 Inbox/Question Log.md`
- active project notes

### Bills And Money

Show:

- Upcoming bills
- Recurring bills
- Subscriptions to review
- Insurance renewals
- Links to related documents

Sources:

- `20 Areas/Household/Finance/Bills.md`
- `20 Areas/Household/Finance/Subscriptions.md`
- `20 Areas/Household/Finance/Insurance.md`
- `50 Documents/Documents.md`

### Maintenance Radar

Show:

- Open maintenance items
- Recent maintenance log entries
- Room hotspots
- Contractor links
- Seasonal checks

Sources:

- `20 Areas/Household/Maintenance/Maintenance.md`
- `20 Areas/Household/Maintenance/Maintenance Log.md`
- `20 Areas/Household/Maintenance/Contractors.md`
- room notes under `20 Areas/Household/Maintenance/Rooms/`

### Family Logistics

Show:

- School notes
- Health reminders that are safe to display
- Vehicle tasks
- Routines
- Food and meal planning

Sources:

- `20 Areas/Household/School/School.md`
- `20 Areas/Household/Health/Health.md`
- `20 Areas/Household/Vehicles/Vehicles.md`
- `20 Areas/Household/Routines/Routines.md`
- `20 Areas/Household/Food/Meal Planning.md`

### Projects

Show active projects with:

- Status
- Owner
- Next action
- Target date
- Link to project note

Source:

- `10 Projects/Projects.md`

### Emergency Strip

A quiet but easy-to-find emergency section.

Show:

- Emergency plan link
- Contacts link
- Shutoffs link

Do not expose sensitive details unless the user asks.

Sources:

- `20 Areas/Household/Emergency/Emergency.md`
- `20 Areas/Household/Emergency/Contacts.md`
- `20 Areas/Household/Emergency/Shutoffs.md`

### Recent Learning

Show the latest useful entries from `02 Inbox/Question Log.md`.

Use this to surface:

- Questions that revealed missing information
- Notes recently updated
- Follow-up actions

### Documents To File

Show reminders for:

- Inbox items to process
- Receipts or bills awaiting filing
- Documents without dates or clear names

Sources:

- `02 Inbox/To Process.md`
- `50 Documents/Documents.md`

## Visual Direction

Make it feel like a practical household operations board, not a marketing page.

Design preferences:

- Dense but calm layout.
- Clear cards or panels, but no nested cards.
- Use a restrained palette with several distinct status colors.
- Use compact typography.
- Make it responsive for desktop and mobile.
- Use familiar symbols for status: due, waiting, blocked, done, urgent.
- Keep emergency links visible without making the whole dashboard feel alarming.

Suggested status colors:

- Urgent: red
- Due soon: amber
- Waiting: blue
- Done or healthy: green
- Reference only: neutral

## Build Rules

- Save the file as `60 Dashboards/Household Dashboard.html`.
- Keep it self-contained unless the user asks for dynamic file loading.
- Include source-note links near each section.
- Do not invent real household facts.
- Placeholder content is allowed only when clearly marked as empty state text.
- Prefer readable HTML, CSS, and JavaScript over cleverness.
- If using JavaScript, use it for filtering, collapsing sections, and local UI state only.
- Avoid external CDNs so the dashboard works offline.

## Useful Interactions

Consider adding:

- Section collapse toggles.
- Status filter chips.
- A search box for dashboard items.
- A print-friendly mode.
- A "needs update" marker for empty or stale sections.
- Quick links back to important notes.

## Empty States

Use helpful empty states:

- "No active projects recorded."
- "No upcoming bills recorded."
- "No maintenance items recorded."
- "No recent learning logged."

Do not fill empty sections with made-up household data.

## Maintenance Loop

When updating the dashboard:

1. Read `INDEX.md`.
2. Read this instruction file.
3. Read the relevant source notes.
4. Update source notes first if information is missing or stale.
5. Regenerate or edit `Household Dashboard.html`.
6. Add a short `02 Inbox/Question Log.md` entry if the dashboard work revealed a meaningful gap.

## Automatic Refresh After Major Updates

Whenever a major knowledgebase update happens, the dashboard should be checked and refreshed.

Major updates include:

- Importing, moving, or reorganizing household records.
- Updating current priorities.
- Adding or changing active projects.
- Updating bills, subscriptions, insurance, renewals, or document indexes.
- Updating maintenance tasks, contractor information, rooms, utilities, or household systems.
- Updating emergency, school, health, vehicle, people, food, or routine notes.
- Processing multiple inbox items.
- Changing the vault structure or root instructions.

Preferred workflow:

1. Finish the source-note update first.
2. Identify which dashboard sections are affected.
3. If the assistant supports subagents, delegate a dashboard-refresh task to a subagent.
4. The subagent should read `INDEX.md`, this file, and the changed notes.
5. The subagent should update `Household Dashboard.html` if it exists.
6. The subagent should report changed files, stale sections, and any missing source data.
7. If subagents are not available, the active assistant should do the same refresh directly.

Suggested subagent prompt:

```text
You are the dashboard refresh subagent for this household second brain. Read INDEX.md and 60 Dashboards/Household Dashboard Instructions.md. Inspect the notes changed by the parent task. Refresh 60 Dashboards/Household Dashboard.html so it reflects the current Markdown source notes. Do not invent household data. Preserve sensitive information boundaries. Report files changed, sections updated, and any gaps or follow-up actions.
```

If `Household Dashboard.html` has not been built yet, do not create it unless the user asked for dashboard creation. Instead, report that the dashboard does not exist yet and whether the dashboard instructions need updating.
