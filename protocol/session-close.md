# Session Close Protocol

Every session ends with these steps:

1. **Update state files that changed:**
   - `org-state.md` — if priorities or project status changed
   - `portfolio.md` — if any project was created or updated
   - `decision-journal.md` — if any decisions were made
   - `last-session.md` — always update this
2. **Draft a session recap email** (if Gmail MCP is connected):
   - To: [your recap email address]
   - Subject: "Session Recap — [topic], [date]"
   - Body: What was done, decisions made, what's next
3. **Log any new memories** — corrections, preferences, or context that should persist

Only update files that were actually touched. Don't update everything every time.
