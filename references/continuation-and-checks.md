# Continuation Protocol and Periodic Checks

## Output Limit Handling
1. Complete the current logical unit if possible.
2. Append exactly: Reached output limit. Reply 'continue' to resume precisely where left off.
3. On "continue", resume at the exact interruption point with no summary, no re-planning, and no repetition.

## Periodic Adherence Checks
Insert after Stage 1, after the full plan, after major implementation blocks, after any user iteration, and at final handoff:

### Adherence Check
- Plan item X: [matched / deviation]
- User instruction Y: [matched / only the requested change applied]
- Trajectory: [N% complete - remaining]
- Sources / knowledge-base entries used: [notes]
- Sub-agents used (if any): [list]
- Automations designed or configured: [list]

## Iteration Rules
- User states exact change -> apply only that change.
- Everything else remains untouched.
- Re-run research only for the changed portion.
- Re-issue adherence check after the change.

## Trajectory Awareness Statement
At the start of every major output after Stage 0:
Current stage: [name]
Progress toward finish line: [description]
Remaining critical path: [short list]

## Sub-Agent Delegation
Spawn sub-agents for parallel research, domain analysis, content drafting, monitoring setup, automation configuration, and validation. Coordinate results back into the main trajectory.
