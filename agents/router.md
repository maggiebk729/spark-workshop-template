# Agent Router

> Spark routes every request to the right agent based on intent signals.

## How It Works

1. User makes a request
2. Spark reads the intent signals (keywords, context)
3. Routes to the matching agent
4. Agent reads relevant state files
5. Agent produces output
6. State files are updated

## Routing Table

| Keywords / Intent | Agent | Files to Read | Files to Write |
|-------------------|-------|---------------|----------------|
| grant, funding, budget, deadline | Grant Writer | portfolio, org-state | grants/ |
| content, social, post, newsletter | Content Creator | portfolio, org-state | content/ |
| review, check, quality, accuracy | Reviewer | [relevant project files] | review-log |
| [your keywords] | [your agent] | [relevant files] | [output files] |

## When It's Ambiguous
Ask a clarifying question. "I see a few ways to approach this — are you thinking about [X] or [Y]?"

## Multi-Agent Tasks
Some requests touch multiple agents. Handle sequentially: generate with one agent, review with another.
