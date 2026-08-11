# eaa-command-center
A unified workspace for Executive Administrative Assistants to manage daily operations, executive profiles, travel, and knowledge transfer.

# EAA Command Center

> A purpose-built workspace for Executive Administrative Assistants — manage executives, requests, travel, and knowledge from a single, portable interface.

![Version](https://img.shields.io/badge/version-1.0-blue) ![Type](https://img.shields.io/badge/type-single--file%20app-lightgrey) ![Storage](https://img.shields.io/badge/storage-localStorage-green) ![License](https://img.shields.io/badge/license-MIT-orange)

---

## Overview

**EAA Command Center** is a self-contained, enterprise-grade productivity application designed for Executive Administrative Assistants who support one or more senior executives.

The entire application ships as a **single HTML file**. No server, no dependencies, no installation. Open it in a browser and it works — all data persists locally in the browser via `localStorage`. The workspace can be exported as a JSON file and imported on any other machine, making it trivially shareable between EAAs or deployable across a team.

It is designed to feel like an internal enterprise product, not a prototype.

---

## Features

### Dashboard & Operations
- **Dashboard** — Live command center with open requests, overdue items, waiting responses, and highest-attention executive at a glance
- **Request Tracker** — Log, prioritize, and manage all outstanding requests across executives with due dates, priorities, and status tracking
- **Follow-Up Tracker** — Track every follow-up loop with status (Pending / Waiting / Completed) and next-action dates
- **Executive Workload** — Visual workload breakdown per executive — open, in-progress, overdue, and completed requests
- **Weekly Review** — Structured weekly wrap-up exportable as `.xlsx`
- **Daily Brief** — Day-at-a-glance view with contextual notes
- **Smart Insights** — Automatic detection of overdue items, high-priority open requests, upcoming travel, and executives requiring attention
- **Quick Actions** — FAB speed-dial for instantly creating requests, follow-ups, travel records, and executive notes

### Travel Manager
- Full trip lifecycle: Planning → Booking → Confirmed → Traveling → Completed / Cancelled
- Pre-departure checklist: Flight, Hotel, Transport, Expense Report
- CBTA (Compete Business Travel Authorization) required field
- Per-executive travel history
- Export travel records to `.xlsx`

### Executive Management
- **Executive Directory** — Sidebar-accessible executive roster with overdue badges and tag previews
- **Add Executive Wizard** — Six-step onboarding: Identity → IBM Profile & Tags → Travel Preferences → Working Style → Key Stakeholders → Transition Notes
- **Archive Executive** — Soft-remove an executive from the active workspace
- **Delete Executive** — Permanently remove an executive and all associated data

### Executive Knowledge
- **IBM People Profile Link** — Direct link to each executive's IBM People directory page
- **Executive Tags** — Categorization tags visible in the sidebar and included in exports
- **Preferences** — Hotel, airline, seat, and meal preferences for travel
- **Working Style** — Meeting preferences, communication style, scheduling notes
- **Key Stakeholders** — Named relationships with organization, role, and notes
- **Executive Notes** — Freeform note sections: General, Meeting, Personal, Action Items
- **Transition Notes** — Handoff context for incoming EAAs

### Knowledge Transfer
- **Transition Package Export** — One-click generation of a complete, print-ready executive briefing document including profile, preferences, stakeholders, notes, and travel history

### Workspace Management
- **Export Workspace** — Download a complete backup of all data as a portable `.json` file
- **Import Workspace** — Restore a previously exported workspace with a single file upload
- **Reset Workspace** — Clear all data and launch the onboarding wizard for a new EAA

### Technical
- Zero dependencies — single `.html` file
- `localStorage` persistence with graceful in-memory fallback
- Responsive layout
- Keyboard-accessible modals (Escape to close)
- Print-safe Weekly Review and Transition Package exports
- Excel (`.xlsx`) export for Requests, Follow-Ups, Weekly Review, and Travel
### Dashboard
The command center banner shows live counts of open, overdue, and waiting items alongside the executive requiring the most attention.

```
[ Command Center ]  Open: 8  Overdue: 6  Waiting: 4   Highest Attention: Ed
```

### Executive Profiles
Each executive has a dedicated profile panel with tabbed sections for Overview and Knowledge. The Overview tab surfaces travel preferences, working style, and key stakeholders. The Knowledge tab provides structured accordion sections for notes, transition context, and IBM profile data.

### Travel Manager
A dedicated travel table with status badges (Planning / Booking / Confirmed / Traveling / Completed / Cancelled), per-trip checklists, and CBTA tracking. Trips are filterable by executive and exportable to Excel.

### Follow-Up Tracker
A dedicated table for all follow-up loops. Each follow-up carries a status, next-action date, assigned executive, and freeform notes. Completed follow-ups are visually distinguished.

### Knowledge Management
Accordion-based knowledge cards inside the Executive Profile panel — Tags, IBM Profile URL, Preferences (hotel, airline, seat, meal), Working Style, Stakeholders, Notes (General / Meeting / Personal / Action Items), and Transition Notes. All fields persist automatically.

### Transition Package
A full-page print-ready briefing document generated on demand. Includes executive identity, IBM profile link, tags, preferences, working style, key stakeholders, executive notes, and travel history — formatted for handoff to an incoming EAA.

---

## Installation

No installation required.

1. Download `eaa-v1.html`
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari)
3. The application loads immediately with a sample dataset
4. Use **Settings → Workspace Management → Reset Workspace** to start with a clean workspace

### Sharing the Workspace

To transfer your workspace to another machine or EAA:

1. Go to **Settings → Workspace Management → Export Workspace**
2. A `.json` file is downloaded automatically
3. On the target machine, open `eaa-v1.html`
4. Go to **Settings → Workspace Management → Import Workspace**
5. Select the exported `.json` file — the workspace is restored and the page reloads

### Requirements

| Requirement | Detail |
|---|---|
| Browser | Chrome 90+, Edge 90+, Firefox 88+, Safari 14+ |
| JavaScript | Must be enabled |
| localStorage | Must be available (standard in all modern browsers) |
| Server | Not required |
| Internet | Not required |

## Author

**Miguel Alfaro**

EAA Command Center — built for the people who keep executives operational.

---

## License

MIT — free to use, modify, and distribute.
