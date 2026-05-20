# shi-fu

A beginner-friendly routing and translation layer for Matt Pocock's skills. This is not a coding skill — it's a guide that helps non-engineers understand where they are in a project and which skill to use next.

## What this is

shi-fu reads the user's current state (via questions), maps it to one of Matt Pocock's skills, and explains in plain language why that skill is appropriate. It does not execute any engineering tasks itself.

## Skills

- `shi-fu/` — The main skill file

shi-fu is designed to be used alongside `mattpocock/skills`. It assumes those skills are available in the session.

## Key concepts

shi-fu uses a state map to route users to the right skill:

| User state | Recommended skill |
|---|---|
| Has a vague idea | `/grill-me` |
| Has a clear idea, hasn't started | `/grill-me` |
| Working with existing code | `/grill-with-docs` |
| Needs to plan and break into tasks | `/to-prd` then `/to-issues` |
| In the middle of building | `/zoom-out` |
| Something broke | `/diagnose` |
| Wants to make it better | `/improve-codebase-architecture` |
| Wants to write tests | `/tdd` |
