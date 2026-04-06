# Session Start Protocol

Every session begins with these steps:

1. **Read `state/last-session.md`** — instant context from the previous session
2. **Read `state/org-state.md`** — current priorities and deadlines
3. **Check for stale data:**
   - Any file not updated in 7+ days? Flag it.
   - Any deadline within 7 days? Surface it.
4. **Check for contradictions:**
   - Does portfolio status match what org-state says?
   - Are there decisions in the journal that haven't been acted on?
5. **Report:** Brief the founder on what's current, what's stale, and what's urgent.

If the founder just says "hey" or "what's up" — run this protocol and give them the briefing.
