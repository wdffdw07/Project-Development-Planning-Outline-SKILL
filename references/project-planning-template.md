# Project Planning Templates

## Overall Planning Outline

Use this for multi-module projects, platform work, refactors, product initiatives, or multi-week engineering plans.

```markdown
# [项目名称] 开发规划纲要

> **For agentic workers:** REQUIRED: Use superpowers:subagent-driven-development if available, or superpowers:executing-plans to implement this plan. Steps use checkbox syntax for tracking.

**规划周期:** [YYYY-MM-DD 至 YYYY-MM-DD]
**规划性质:** [项目级 / 平台级 / 架构治理 / 迁移工程 / 产品能力建设]
**Goal:** [One sentence describing what this builds]
**Architecture:** [2-3 sentences about the technical approach]
**Tech Stack:** [Key technologies/libraries]

---

## 一、规划背景与依据

[说明项目为什么做、依据什么上位目标、覆盖什么范围、规划周期多长。]

## 二、现状基础与主要问题

[说明已有功能、代码基础、可复用能力、主要短板、技术债和风险点。]

## 三、形势判断与需求分析

[说明用户场景、业务变化、技术趋势、外部依赖、约束条件和不确定性。]

## 四、总体要求

[写设计原则、工程原则、用户体验原则、非目标和决策边界。]

## 五、主要目标与指标体系

### 约束性目标

- [必须满足的验收条件]

### 预期性目标

- [希望改善的指标或能力]

## 六、重点任务

### [完善/优化/健全/构建][对象]，[提升/支撑/保障][结果]

**目标:** [任务目标]
**范围:** [任务边界]
**措施:** [主要措施]
**交付物:** [具体 deliverables]
**验收标准:** [acceptance criteria]

## 七、系统布局与阶段安排

### 系统布局

[模块边界、数据流、架构关系、用户流程或团队分工。]

### 阶段安排

- 第一阶段：[基础建设]
- 第二阶段：[能力接入]
- 第三阶段：[验证发布]

## 八、重大工程与交付物

### 专栏 1：[核心能力建设工程]

- [deliverable 1]
- [deliverable 2]

## 九、实施保障

- 责任落实：[owner, review, decision process]
- 资源保障：[dependencies, access, data, environments]
- 测试保障：[unit, integration, e2e, regression]
- 发布保障：[feature flag, rollout, rollback]
- 风险防控：[risks and mitigations]

## 十、监测评估与调整机制

- 进度监测：[cadence and signal]
- 指标评估：[metrics and thresholds]
- 中期评估：[when to review]
- 调整机制：[when and how to revise the plan]

---

# Implementation Tasks

[Use the implementation task layer when execution is expected.]
```

## Special Plan

Use this for frontend, backend, data, security, testing, deployment, UX, migration, or architecture domains.

```markdown
# [领域名称]专项开发规划

## 一、专项定位

[说明本专项服务哪个总体规划，解决哪个领域问题。]

## 二、现状与短板

[该领域已有基础和主要问题。]

## 三、专项目标

### 约束性目标
- [...]

### 预期性目标
- [...]

## 四、重点任务

### [任务标题]

**目标:**
**措施:**
**交付物:**
**验收标准:**

## 五、与总体规划的衔接

[说明该专项如何服务总体目标，和其他专项如何协同。]

## 六、实施保障与评估

[测试、发布、owner、风险、评估。]
```

## Implementation Scheme

Use this for one feature, milestone, migration batch, or bugfix campaign.

```markdown
# [功能/里程碑名称]实施方案

## 一、实施背景

[当前问题和为什么现在实施。]

## 二、实施目标

- 约束性目标：[must-pass]
- 预期性目标：[desired]

## 三、实施范围

### Included
- [...]

### Excluded
- [...]

## 四、文件结构与模块边界

- Create: `path/to/file`
- Modify: `path/to/file`
- Test: `path/to/test`

## 五、实施步骤

[Use exact checkbox tasks.]

## 六、测试与验收

[Commands, expected output, manual checks.]

## 七、发布与回滚

[Rollout, migration, rollback.]
```

## Assessment Report

Use this after a milestone, launch, or plan revision.

```markdown
# [项目名称]规划实施评估报告

## 一、评估范围

[Which plan, which period, which deliverables.]

## 二、目标完成情况

| 目标 | 状态 | 证据 | 说明 |
| --- | --- | --- | --- |

## 三、重点任务完成情况

[Completed, partial, blocked.]

## 四、主要问题与原因

[Issues and causes.]

## 五、调整建议

[Continue, revise, stop, split, or add safeguards.]

## 六、后续安排

[Next plan or implementation tasks.]
```

