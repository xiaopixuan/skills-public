# Skill Design Review Rubric

Score each criterion from 0 to 2.

| Criterion | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Skill necessity | Skill duplicates baseline agent ability, overlaps heavily with another skill, or adds context cost without measurable lift. | Skill has some durable value, but the keep/simplify/merge/delete decision is ambiguous or weakly evidenced. | Skill clearly provides durable value beyond baseline: domain knowledge, tool/script routing, stable output standards, organizational memory, or measured quality lift. |
| Trigger behavior | Description misses likely user requests, uses vague scope, or would not trigger when needed. | Description covers the main case but misses common phrasing, related contexts, or over-triggers. | Description clearly states what the skill does and when to use it, including realistic trigger phrases and boundaries. |
| Workflow guidance | SKILL.md gives generic advice without an executable sequence. | SKILL.md has a sequence, but leaves important decisions or validation steps implicit. | SKILL.md gives a clear, ordered workflow with decision points and enough constraints to guide execution. |
| Output format | Expected output is absent, unstable, or mismatched to the user's likely need. | Output format exists but lacks required fields, order, or evidence requirements. | Output format is explicit, stable, and produces a reusable artifact or clear user-facing result. |
| Content quality | Instructions are misleading, bloated, contradictory, or omit essential domain knowledge. | Instructions are mostly correct but include noise, weak examples, or missing edge cases. | Instructions are concise, accurate, context-efficient, and include the non-obvious details needed for repeatable quality. |

## Evidence Requirements

For every score below 2, cite the specific phrase, missing instruction, failed behavior, or output mismatch that caused the deduction.

For every proposed fix, state which test case or criterion it is expected to improve.

## Suggested Test Case Pattern

Use this compact format:

```markdown
### Test Case A: Ordinary request
User request:
Input artifact/context:
Expected output shape:

### Test Case B: Edge or ambiguous request
User request:
Input artifact/context:
Expected output shape:
```

## Scorecard Template

```markdown
| Criterion | Score | Evidence | Fix |
| --- | ---: | --- | --- |
| Skill necessity | /2 |  |  |
| Trigger behavior | /2 |  |  |
| Workflow guidance | /2 |  |  |
| Output format | /2 |  |  |
| Content quality | /2 |  |  |
| Total | /10 |  |  |
```

## Re-run Note

After a revision, re-score only the affected criterion unless the patch changes the skill's overall workflow. Record the before and after score.
