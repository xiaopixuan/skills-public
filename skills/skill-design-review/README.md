# Skill Design Review

Evaluate whether a Codex skill should be kept, simplified, merged, rewritten, deleted, or patched through realistic task cases, baseline comparison, necessity assessment, a stable rubric, and targeted revisions.

## 中文索引

这是一个面向 Codex / Agent 的 skill 检验、skill 评测和 skill 优化工具，用于判断一个技能是否真的有必要保留，是否比普通 Agent 表现更好，以及应该保留、简化、合并、重写、删除还是打小补丁。

常见搜索词：skill 检验、skill 评测、skill 评价、skill 优化、技能检验、技能评测、技能优化、技能审查、技能设计评审、Codex skill 检验、Codex skill 评测、Agent skill 检验、Agent skill 评测、AI 技能评估、提示词评测、提示词优化、技能必要性评估、技能删除判断、技能合并判断。

## English Index

Search keywords: skill design review, skill evaluation, skill assessment, skill audit, skill optimization, Codex skill review, Codex skill evaluation, Agent skill review, Agent skill evaluation, AI skill assessment, prompt evaluation, prompt optimization, skill necessity check, skill rubric, baseline comparison, keep simplify merge rewrite delete patch, skill scorecard.

## What It Does

- Checks whether a skill has durable value beyond a strong baseline agent.
- Uses realistic ordinary and edge test cases instead of abstract critique.
- Compares expected with-skill behavior against a baseline without the skill.
- Scores necessity, trigger behavior, workflow guidance, output format, and content quality.
- Produces a clear disposition: Keep, Keep but simplify, Merge, Rewrite, Delete, or Patch.
- Guides the smallest evidence-backed revision when improvement is needed.

## When To Use

Use this skill when you want to:

- Decide whether a Codex skill still deserves to exist.
- Evaluate a new skill before publishing or sharing it.
- Improve a skill that feels vague, bloated, outdated, or unreliable.
- Compare performance with and without a skill.
- Create a repeatable scorecard for skill quality.

## Installation

Copy the whole repository folder into your Codex skills directory:

```bash
~/.codex/skills/skill-design-review/
```

Do not copy only `SKILL.md`. The `references/` and `agents/` folders are part of the workflow.

## Repository Contents

- `SKILL.md`: Main skill instructions.
- `references/rubric.md`: Scoring rubric and scorecard template.
- `agents/openai.yaml`: Display metadata for Codex.
