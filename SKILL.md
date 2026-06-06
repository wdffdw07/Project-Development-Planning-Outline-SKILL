---
name: project-development-planning-outline
description: Create project development planning documents in the style of formal Chinese planning outlines, adapted for software engineering. Use when Codex needs to write or revise project planning, implementation plans, feature plans, technical special plans, architecture plans, migration plans, roadmap documents, milestone plans, or post-plan assessment reports using a layered system of overall planning outline, special plans, implementation schemes, task checklists, metrics, safeguards, and evaluation mechanisms.
---

# Project Development Planning Outline

## Overview

Use this skill to turn product or engineering requirements into a formal but executable planning document system. Combine the discipline of Chinese official planning documents with agentic software planning practices.

This skill replaces or augments only the planning-document-writing role of `superpowers:writing-plans`. It does not replace brainstorming, TDD, execution, debugging, verification, review, or branch-finishing skills. When implementation starts, hand off to the appropriate execution and verification skills.

## Workflow

1. Determine the planning level:
   - Overall planning outline: multi-week/multi-module project, product initiative, platform build, large refactor.
   - Special plan: frontend, backend, data, testing, security, deployment, migration, architecture, UX.
   - Implementation scheme: one feature, milestone, migration batch, bugfix campaign, or release.
   - Assessment report: after delivery, milestone review, launch review, or plan adjustment.
2. Read `references/official-style.md` for language patterns and planning document habits.
3. Read `references/project-planning-template.md` for document templates and section order.
4. If the plan will be executed by Codex/agents, include the implementation task layer from `references/implementation-layer.md`.
5. Inspect the codebase before writing executable tasks. Exact file paths and commands are required for implementation plans.
6. Write the plan as a layered system when the project is complex:
   - `project-plan.md` for the overall outline.
   - `plans/special-*.md` for domain-specific plans.
   - `plans/implementation-*.md` for executable schemes.
   - `plans/assessment-*.md` for reviews and adjustments.
7. Keep official style useful, not performative. Use formal planning language to clarify hierarchy, goals, indicators, and responsibility; use engineering language for files, tests, commands, and code.

## Required Structure

For an overall project planning outline, use this order:

1. Planning background and basis
2. Current foundation and main problems
3. Situation judgment and demand analysis
4. Overall requirements
5. Main objectives and indicator system
6. Key tasks
7. System layout and phased arrangement
8. Major projects and deliverables
9. Implementation safeguards
10. Monitoring, evaluation, and adjustment mechanism
11. Implementation tasks, if execution is expected

For a special plan, narrow the same structure to one domain. For an implementation scheme, start with scope, files, tasks, tests, release, and rollback.

## Style Rules

- Prefer section titles shaped as "verb + object + outcome", such as "完善认证链路，提升登录稳定性".
- For task paragraphs, use three moves: direction sentence, measure sentence, result sentence.
- Use planning verbs precisely: 坚持, 完善, 健全, 优化, 强化, 提升, 推进, 加快, 构建, 形成, 夯实, 规范, 统筹.
- Split goals into binding goals and expected goals:
  - Binding goals: must-pass acceptance criteria.
  - Expected goals: desired improvements or directional metrics.
- Separate "what to do" from "how to ensure it gets done".
- Explicitly state non-goals and boundaries to prevent uncontrolled scope.
- Keep the final document executable: every implementation task needs exact paths, tests, commands, expected output, and a completion/commit step.

## Output Decision

If the user asks for "规划", "纲要", "plan", or "planning" without more detail, produce an overall planning outline plus an implementation task appendix.

If the user asks for a concrete feature or bugfix plan, produce an implementation scheme but include a concise official-style opening: background, current problem, objective, and safeguards.

If the user asks to "make it official/formal", strengthen the planning language but keep code steps concrete.

## References

- `references/official-style.md`: official planning language habits, sentence patterns, and verbs.
- `references/project-planning-template.md`: templates for overall outlines, special plans, implementation schemes, and assessment reports.
- `references/implementation-layer.md`: engineering execution layer adapted from superpower planning.

