# Requirements: Festa, GenAI Event Planning Assistant

## 1. Problem
Organising a wedding, birthday or community event means juggling budgets, deadlines and vendors, usually across scattered notes and chats. People overspend, miss bookings and run short of ideas.

## 2. Goal
A single-page assistant that turns a few inputs into a complete, practical event plan and gives personalised AI ideas.

## 3. Users
- Families planning weddings and birthdays
- Community groups, resident associations, clubs and student teams
- Freelance or first-time event planners

## 4. Functional requirements
| ID | Requirement |
|----|-------------|
| FR1 | User selects event type: wedding, birthday or community event |
| FR2 | User enters guest count, total budget (INR), event date, and optional theme or constraints |
| FR3 | System shows a budget split by category with amounts, percentages and per-guest cost |
| FR4 | System shows a timeline of milestones counted back from the event date, with calendar dates |
| FR5 | System shows a vendor checklist per event type with a progress counter |
| FR6 | Vendor ticks persist across page reloads on the same browser |
| FR7 | AI generates 8 personalised ideas from the inputs (theme, decor, food, entertainment, savings, guest experience) |
| FR8 | User can ask the AI free-form planning questions and see streamed answers |
| FR9 | Plan features (FR3-FR6) work without AI |

| FR10 | A demo walkthrough shows the app in 8 captioned scenes with play, pause and navigation |
| FR11 | Demo offers optional voice narration and background music, off by default, with scenes waiting for narration to finish |
| FR12 | One project hub page presents index.html, requirements.md, readme.md, tasks.md and the version history |

## 5. Non-functional requirements
- Single self-contained `index.html`, no build step
- Responsive from phone to desktop; light and dark themes
- AI failures or declined permission degrade gracefully with a clear message
- All AI output is rendered as plain text (no HTML injection)
- No personal data leaves the browser except the prompt sent to the AI

## 6. AI design
- Prompt includes event type, guests, budget, date, notes and an India-default audience
- Ideas call requests a strict JSON array of `{title, detail}` objects
- Q&A call asks for concise plain-text answers under 120 words

## 7. Out of scope (v1)
Guest list and RSVP tracking, real vendor marketplace, payments, multi-user collaboration, actual-spend tracking.

## 8. Success criteria
- A user gets a full plan in under one minute
- Budget percentages always total 100%
- Page works with AI unavailable
