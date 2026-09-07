# GrokBot GTM Agent System

A source-bound starter repository for building and operating a small GTM bot team in GrokBot.

## Start here

1. Read `GROKBOT.md`.
2. Fill out `workspace/context.md` and `workspace/voice.md`.
3. Start with the three Level 1 bots in `bots/`.
4. Run each bot manually before scheduling anything.
5. Promote work using: Task -> 3 clean runs -> Skill -> 5 clean runs -> Routine.
6. Keep durable state in `workspace/` files. One owner per state file.
7. Never let a bot send, publish, purchase, delete, sign, or write to CRM without explicit human approval.

## Repo structure

```text
GROKBOT.md                    Master operating instructions
bots/                         Starter bot specs
templates/bot-spec.md         Reusable six-block bot template
templates/run-review.md       Manual run QA checklist
workspace/context.md          Your GTM context
workspace/voice.md            Voice rules and NEVER list
workspace/signals.md          Signal Watcher state
workspace/deals.md            Deal Desk state
workspace/prospects/          Prospect queue and completed accounts
workspace/accounts/           Named-account knowledge files
docs/30-day-rollout.md        Rollout plan
docs/fleet-governance.md      Guardrails, silent failures, kill rules
```

## Recommended first three bots

- Chief of Staff
- Meeting Prep
- Call Follow-Up Drafter

Do not create routines on day one.
