# Festa: GenAI Event Planning Assistant

Plan weddings, birthdays and community events with budgets, timelines, vendor checklists and personalised AI ideas, all in one HTML file.

## Features
- **Budget planner:** category split, amounts in INR, per-guest cost, built-in contingency
- **Timeline:** milestones back-calculated from your event date
- **Vendor checklist:** per event type, with progress and saved ticks
- **AI ideas and Q&A:** personalised suggestions and free-form planning advice

## Files
| File | Purpose |
|------|---------|
| `index.html` | The complete app (HTML, CSS, JS) |
| `requirements.md` | Problem, users, functional and non-functional requirements |
| `readme.md` | This file |
| `tasks.md` | Build plan and status |

## How to use
1. Open the deployed link.
2. Choose the event type and enter guests, budget, date and any theme or constraints.
3. Press **Build my plan**, then browse the Budget, Timeline and Vendors tabs.
4. Open **Ideas** to generate AI suggestions or ask a question.

## Tech
Vanilla HTML, CSS and JavaScript. AI features use the Claude runtime available on the hosted page. Local storage saves vendor progress.

## Running elsewhere
The plan tabs work anywhere. The AI tab needs a host that provides the `claude.use("sample")` runtime; on other hosts it shows a friendly "unavailable" message. To use another LLM, replace the `ideas()` and `ask()` functions with a call to your own API.

## Version history
| Version | Change |
|---------|--------|
| v1.0 | `index.html`: Festa app with input form, Budget, Timeline, Vendors and AI Ideas/Q&A tabs |
| v1.1 | Added `requirements.md`, `readme.md` and `tasks.md` to complete the four-file deliverable |
| v1.2 | Demo walkthrough page: 8 auto-advancing scenes with captions and controls |
| v1.3 | Demo sound: voice narration, background music, narration-synced scenes, pause/resume for audio, wrapping controls |
| v1.4 | Single project hub link presenting all four files and the version history |

## Deployed links
- App: https://claude.ai/artifact/DLSBQ9rL3mJVttUmWu3kcW
- Video: https://claude.ai/artifact/EpfcsAAgqL9pq5UuAczZre
- Project hub (all four files + version history): https://claude.ai/artifact/5KeWeWKk6jUiEuuicCjfkU
- MVP (PDF): _add link_

## Author
Gundluru Rajasekhar
