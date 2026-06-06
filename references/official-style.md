# Official Planning Style for Project Development

## Core Writing Rhythm

Formal planning documents usually proceed in this order:

1. Define the document's nature and role.
2. Review existing foundation and progress.
3. Identify problems and constraints.
4. Judge the situation and future demand.
5. State overall requirements and principles.
6. Set goals and indicators.
7. Organize key tasks.
8. Define layout, projects, safeguards, monitoring, and adjustment.

For software planning, preserve this rhythm but replace policy content with product, architecture, delivery, and quality content.

## Opening Formulas

Use these sparingly and adapt them to real context:

- 本规划是……的项目级开发规划，主要阐明……，是后续开发、测试、发布和复盘的重要依据。
- 本方案围绕……，明确目标任务、实施路径、责任边界和验收机制。
- 本阶段是……由……向……转变的关键阶段。
- 本专项规划聚焦……，用于指导……领域的能力建设和任务落地。

Example:

```markdown
本规划是用户认证链路稳定性治理的一期开发规划，主要阐明系统改造目标、模块边界、重点任务、实施路径和验收机制，是后续开发、测试、发布和复盘的重要依据。
```

## Current-State Formulas

Official style often balances progress with problems:

- ……取得积极进展，但……仍然突出。
- ……基础不断夯实，但……短板仍需补齐。
- ……总体运行平稳，但……深层次问题尚未根本解决。
- ……已支撑主要业务流程，但……影响后续扩展和稳定运行。

Example:

```markdown
当前订单模块已支撑主要交易流程，接口结构和业务链路基本稳定，但仍存在状态流转分散、异常处理不一致、测试覆盖不足等问题，影响后续扩展和故障定位效率。
```

## Planning Verbs

Use verbs by intent:

| Verb | Meaning | Software planning use |
| --- | --- | --- |
| 坚持 | Set a principle | 坚持接口兼容、渐进迁移 |
| 完善 | Improve an existing thing | 完善测试覆盖、完善错误处理 |
| 健全 | Build or complete a mechanism | 健全发布回滚机制 |
| 优化 | Improve structure, flow, or performance | 优化查询链路 |
| 强化 | Increase constraint or capability | 强化权限校验 |
| 提升 | Improve measurable outcome | 提升加载性能 |
| 推进 | Carry forward a task | 推进模块迁移 |
| 加快 | Increase pace | 加快关键路径改造 |
| 构建 | Build a system from scratch | 构建统一日志体系 |
| 形成 | Reach a stable end state | 形成标准化接入流程 |
| 夯实 | Strengthen the foundation | 夯实数据模型基础 |
| 规范 | Standardize behavior | 规范接口返回结构 |
| 统筹 | Coordinate multiple concerns | 统筹前后端接口变更 |

## Section Title Pattern

Prefer "verb + object + outcome":

- 完善认证链路，提升登录稳定性
- 优化数据结构，支撑订单状态统一管理
- 健全测试体系，保障核心流程稳定上线
- 构建监控告警机制，提升故障发现和处置能力
- 规范模块边界，降低跨域变更风险

Avoid bare labels like "登录", "数据库", "测试", or "后端".

## Task Paragraph Pattern

Use three moves:

1. Direction sentence: what to advance.
2. Measure sentence: concrete measures.
3. Result sentence: capability or state to form.

Example:

```markdown
推进订单状态统一治理。梳理现有状态流转路径，合并重复状态判断，建立统一状态枚举和转换规则。形成可测试、可追踪、可扩展的订单状态管理能力。
```

## Goal Pattern

Use "time node + qualitative result + quantitative indicators":

```markdown
到本阶段结束，认证链路稳定性治理取得明显成效，登录、刷新、登出等核心流程形成统一服务入口；登录失败率下降至 0.5% 以下，认证相关单元测试覆盖率达到 85% 以上。
```

Split goals:

- 约束性目标: hard acceptance criteria and must-pass checks.
- 预期性目标: directional improvement targets.

## Safeguard Pattern

Use safeguards to make the plan governable:

```markdown
加强任务责任落实，明确每个工作包的 owner、验收口径和交付时间。强化测试与发布保障，所有核心链路变更须通过单元测试、集成测试和回归验证。健全风险处置机制，对接口兼容、数据迁移和上线回滚制定预案。
```

## Style Boundaries

- Be formal, but never vague.
- Do not replace implementation details with grand language.
- Do not use official wording to hide uncertainty.
- For engineering tasks, include exact file paths, commands, expected results, and acceptance criteria.
- Use Chinese formal style for planning sections; use precise technical English where project conventions require it.

