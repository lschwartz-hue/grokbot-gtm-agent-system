# Fleet Governance

## Five silent failures
1. Connector/credit exhaustion returns zero and masquerades as a quiet day.
2. Page layout changes return empty results and masquerade as no change.
3. Manual context never made it into the bot instruction.
4. Bot memory drifts or becomes stale.
5. Confidence labels inflate because HIGH gets rewarded.

## Required guardrails
- Report every input and its count/fetch status.
- Explicit silence rule.
- Spend-and-send approval boundary.
- Draft-only default for customer-facing work.
- Task -> 3 clean runs -> Skill -> 5 clean runs -> Routine.
- Durable facts live in workspace files, not chat memory.

## File ownership
One owner per state file, always.

## Coordination
- Pass file paths, not pasted payloads.
- Keep coordinator messages short.
- Keep groups at six bots or fewer.

## 14-day kill rule
If a bot or routine has not produced an approved, used, sent, or acted-on output in 14 days, flag it for deletion.

## Usage discipline
Spend agent effort primarily on judgment-heavy work such as deep research and synthesis. Avoid open-ended browsing, unnecessary overnight monitoring, long coordinator conversations, and large deliberative bot groups.
