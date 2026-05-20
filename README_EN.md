# shi-fu (师傅)

A beginner-friendly routing and translation layer for [Matt Pocock's skills](https://github.com/mattpocock/skills).

## What this is

Matt Pocock open-sourced a set of professional engineering skills (/grill-me, /tdd, /diagnose, etc.) — but they assume you already know what a PRD is, what TDD means, and when to debug vs. when to plan.

shi-fu is the **translation layer and routing layer** for this toolkit. It asks a few questions first, identifies which engineering phase you're in, recommends the right skill, and explains it in plain language.

## Who it's for

- People who want to learn engineering but don't know where to start
- People with ideas who don't know which tools to use
- Anyone blocked by engineering jargon and陌生的概念

## How it works

```
You → shi-fu (questions + phase detection + skill recommendation) → Matt Pocock Skill (execution)
```

shi-fu writes no code. It's just a **guide**.

## Quick start

### Step 1: Install Matt Pocock Skills

```bash
npx skills@latest add mattpocock/skills
```

### Step 2: Install shi-fu

```bash
cp SKILL.md ~/.claude/skills/shi-fu/SKILL.md
```

### Step 3: Use it

In Claude Code, just type:

```
/shi-fu
```

Answer the questions. It'll guide you through your project.

## Engineering phase map

| Where you are | Recommended skill | Why |
|---|---|---|
| Vague idea, not sure what you want | `/grill-me` | Figure out what you actually want first |
| Clear idea, haven't started | `/grill-me` | Make sure you're building the right thing |
| Working with existing code | `/grill-with-docs` | Build a shared language with the AI |
| Need to plan and break into tasks | `/to-prd` then `/to-issues` | Write the plan first, then break it down |
| In the middle of building | `/zoom-out` | Step back and see the bigger picture |
| Something broke | `/diagnose` | Debug systematically, not by guessing |
| Want to make it better | `/improve-codebase-architecture` | Tidy up before tangles become problems |
| Want to write tests | `/tdd` | Test first, code second |

## Related

- [Matt Pocock Skills](https://github.com/mattpocock/skills) — the engineering skills本体
- [Matt Pocock Course](https://www.aihero.dev/cohorts/ai-coding-for-real-engineers-m0k0w) — paid course teaching the same workflow