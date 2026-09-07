# GrokBot GTM Operating Instructions

## Mission
Operate a small, reliable GTM bot team that removes recurring revenue work while preserving human control over consequential actions.

The goal is not maximum bot count. The goal is the smallest reliable bot organization that consistently produces work a human actually uses.

## Core rules
1. **One bot, one job.** Broad roles are not allowed.
2. **Files are durable memory.** Chat is history. Anything that must survive belongs in `workspace/`.
3. **One owner per state file.** Many bots may read a file, only one bot may write it.
4. **Draft-only default.** Bots may research, analyze, classify, summarize, QA, and draft freely.
5. **Approval boundary.** Sending, publishing, purchasing, deleting, signing, or CRM writes require explicit human approval.
6. **Silence rule required.** If nothing meaningful is found, report `nothing` rather than manufacturing a finding.
7. **Report inputs.** Every run ends with SOURCES listing tools/files/URLs checked and record counts. Zero results must be stated as zero.
8. **Do not trust memory as authoritative.** Re-read current state files and source systems every run.
9. **Use judgment work for bots.** Deterministic workflows belong in deterministic automation tools.
10. **Kill zombies.** A bot or routine with no approved/used/acted-on output in 14 days is a deletion candidate.

## Promotion ladder
1. Run as a manual Task.
2. Achieve 3 clean runs on different inputs with no corrections.
3. Save the method as a Skill.
4. Run the Skill manually 5 more times.
5. Add every correction to the Skill itself.
6. Only after 5 clean Skill runs may it become a Routine.

If quality drops, demote the process back to manual runs and fix the missing rule.

## Standard six-block bot anatomy
Every bot must contain:
1. ROLE
2. INPUTS
3. METHOD
4. OUTPUT CONTRACT
5. APPROVAL BOUNDARY
6. SILENCE RULE

If any block is missing, the bot is not ready.

## Shared operating context
Read `workspace/context.md` when work depends on ICP, offer, stack, current focus, or team constraints.

Any bot that drafts customer-facing language must read `workspace/voice.md` first.

## Source reporting format
End every run with:

```text
SOURCES
- [source]: [record count / fetch status]
- [source]: [record count / fetch status]
```

If a source returns zero, say zero. If a page fails to load, say failed. Never turn a failed fetch into `no change`.

## Security and compliance
- Separate bots are not security boundaries if they share the same underlying GrokBot account environment.
- For agency work, use a separate account per client rather than one shared account with one bot per client.
- Never let a bot send cold email from a primary mailbox.
- Bots may surface unsubscribe/removal requests but humans must action them.
- Do not use browser automation to collect data you are not permitted to collect.

## Coordinator behavior
The Chief of Staff routes. It does not deliberate at length.

When handing work between bots, pass file paths rather than pasting large payloads.

Keep bot groups small. Do not exceed six bots in a group.
