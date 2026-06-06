# Project Development Planning Outline Skill

为提升 AI 辅助软件开发 planning 阶段的系统性、规范性和可执行性，借鉴正式规划文件的结构安排和表达方式，制定本 Skill。

本 Skill 面向 Codex 及相关 agentic development 场景，聚焦 `superpowers:writing-plans` 所承担的规划文档编写环节，主要用于生成项目开发规划纲要、专项开发规划、具体实施方案和规划实施评估报告，推动项目 planning 从简单任务清单向目标清晰、边界明确、任务可落、结果可评的规划体系转变。

## 一、总体要求

坚持目标导向、问题导向和结果导向，统筹正式规划写法与软件工程实践，围绕项目背景、现状问题、总体要求、目标指标、重点任务、实施保障和评估调整等关键内容，形成可指导开发、测试、发布和复盘的规划文档生成能力。

坚持规划表达与工程落地相衔接，在规划层明确方向、原则、目标和任务，在实施层细化文件路径、测试命令、预期输出、验收标准和提交步骤，保障规划文件既具备总体指导作用，也能够服务后续执行。

## 二、建设目标

到本 Skill 应用成熟阶段，基本形成适用于软件项目开发的多层级 planning 文档体系，项目规划的结构化、可执行化和可评估化水平明显提升。

规划纲要、专项规划、实施方案和评估报告之间的衔接更加清晰；约束性目标和预期性目标的表达更加规范；重点任务、重大工程和阶段安排的组织更加有序；规划内容向 exact files、TDD steps、commands、expected output 和 commit checkpoints 的转化更加顺畅。

## 三、主要任务

### 夯实规划文档编制基础

完善项目开发规划纲要模板，围绕背景依据、现状问题、形势判断、总体要求、目标指标、重点任务、系统布局、实施保障和监测评估等内容，建立适用于复杂软件项目的 planning 文档骨架。

### 推进多层级规划有效衔接

构建总体规划纲要、专项开发规划、具体实施方案和实施评估报告相互衔接的文件体系，支持 frontend、backend、data、security、testing、deployment、migration、architecture 和 UX 等领域形成专项 planning。

### 强化规划任务执行转化

将正式规划中的目标、任务和工程安排转化为可执行的开发步骤，明确文件结构、模块边界、测试验收、发布回滚和风险处置要求，提升规划对实际编码工作的支撑能力。

### 健全评估调整机制

建立规划实施评估报告模板，围绕目标完成情况、重点任务进展、主要问题原因、调整建议和后续安排开展复盘，形成规划编制、实施、评估、调整的闭环。

## 四、组织实施

本仓库以 Skill 文件和参考材料共同构成使用基础：

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── implementation-layer.md
    ├── official-style.md
    └── project-planning-template.md
```

其中，`SKILL.md` 明确触发场景、使用流程和能力边界；`references/official-style.md` 沉淀正式规划文件的语言习惯和句式结构；`references/project-planning-template.md` 提供规划纲要、专项规划、实施方案和评估报告模板；`references/implementation-layer.md` 衔接工程执行层，明确文件路径、测试命令、预期结果和提交步骤。

本 Skill 仅替代或增强 `superpowers:writing-plans` 的规划文档编写职责。进入代码实施阶段后，应继续衔接相应的执行、测试、验证、评审和分支收尾能力，确保规划目标在工程实践中有效落实。
