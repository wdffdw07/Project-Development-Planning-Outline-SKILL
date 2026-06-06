# Project Development Planning Outline Skill

本项目是面向 AI 辅助软件开发流程建设的规划类 Skill，旨在借鉴正式规划文件的结构体系、描述方法和任务分解逻辑，完善项目开发 planning 阶段的文档生成能力，为复杂项目的需求梳理、目标设定、任务拆解、实施保障和评估调整提供规范化支撑。

项目聚焦 `superpowers:writing-plans` 所承担的规划文档编写环节，重点构建“总体规划纲要、专项开发规划、具体实施方案、实施评估报告”相衔接的多层级 planning 体系。通过引入背景依据、现状问题、总体要求、指标体系、重点任务、重大工程、实施保障和监测评估等正式规划写法，推动项目 planning 从简单任务清单向结构清晰、边界明确、可执行、可评估的开发规划转变。

本 Skill 不替代 brainstorming、TDD、debugging、execution、verification、code review 或 branch finishing 等完整开发流程能力，而是作为 planning 阶段的增强模块，在需求明确后生成更系统的项目开发规划，并在实施阶段衔接可执行的文件路径、测试命令、验收标准和任务清单。

## Contents

- `SKILL.md`: Skill trigger, workflow, output rules, and boundaries.
- `agents/openai.yaml`: UI metadata for the skill.
- `references/official-style.md`: Formal planning language patterns and writing habits.
- `references/project-planning-template.md`: Templates for planning outlines, special plans, implementation schemes, and assessment reports.
- `references/implementation-layer.md`: Engineering execution layer adapted from implementation planning practice.

## Intended Use

Use this skill when you need to write or revise:

- Project development planning outlines
- Technical special plans
- Feature or milestone implementation schemes
- Architecture, migration, testing, deployment, or security plans
- Planning assessment and adjustment reports
- Executable implementation checklists connected to a formal plan

## Boundary

This skill replaces or augments only the planning-document-writing role of `superpowers:writing-plans`. When implementation begins, hand off to the appropriate execution, testing, verification, review, and branch-completion skills.
