# Seven Data AI

> AI data engineering, data warehouse delivery, and production-grade Data Agent workflows.

我长期关注一件事：**AI 怎么真正进入数据团队的生产流程**。

不是做一个能演示的聊天框，也不是让大模型随便写几条 SQL。真正有价值的是把企业里已经存在的指标口径、数仓分层、SQL 规则、权限边界、运行日志和业务经验，整理成 AI 可以理解、调用、校验和持续迭代的工程体系。

## What I work on

- **AI + Data Warehouse**
  - ODS / DWD / DWS / ADS 分层设计
  - 交易主题数仓建模
  - 指标口径、字段血缘、质量规则和上线检查

- **Data Agent**
  - AI 问数 / AI 取数
  - NL2SQL / Text2SQL
  - SQL Review / 权限拦截 / 成本控制
  - Agent 运行日志、Bad Case 归因和回归样本沉淀

- **Agent Engineering**
  - Skills / MCP / CLI 工作流
  - Subagent 编排
  - Hooks 生命周期卡点
  - 评测观测与可迭代工程闭环

- **Knowledge Products**
  - AI 数据工程实战知识库
  - 企业 Data Agent 落地案例
  - 数据开发提效模板和方法论

## Current direction

我现在主要在做一套面向数据团队的 AI 工程化方法：

```text
业务问题
  -> 需求澄清
  -> 指标/表/字段/权限匹配
  -> SQL 生成与 Review
  -> 查询执行与结果解释
  -> 运行日志与 Bad Case 归因
  -> 知识资产回流
```

这条链路的目标不是“替代数据开发”，而是把低风险、重复性、可校验的数据工作自动化，同时让复杂数据开发保留工程边界和人工确认。

## Repositories worth watching

### [`ai-dw-workbench`](https://github.com/Rrocean/ai-dw-workbench)

Enterprise-oriented Data + AI workbench.

It covers requirement clarification, warehouse design, controlled database analysis, release gates, governance checks, and knowledge flywheel for Data Agent systems.

### [`data-agent-eval-kit`](https://github.com/Rrocean/data-agent-eval-kit)

Evaluation templates for AI ask-data / fetch-data / NL2SQL workflows.

Focus areas:

- Gold Case design
- baseline SQL
- metric consistency
- SQL review rules
- permission and sensitive field checks
- Bad Case attribution

This is the first public toolkit in this direction. It includes Gold Case templates, trade-domain sample cases, baseline SQL, SQL review rules, a lightweight evaluator and a production readiness checklist.

### `ai-data-skills`

Reusable agent skills for data teams.

Planned skills:

- DWD fact table designer
- SQL reviewer
- metric matcher
- data requirement clarifier
- report evidence checker
- data agent runbook generator

### `sql-review-rules`

Production SQL review rules for AI-generated SQL.

Examples:

- partition filter required
- forbid sensitive fields
- prevent join amplification
- block dangerous DDL/DML
- check metric grain
- check engine-specific syntax

## Writing and content

我也在持续输出中文内容，方向集中在：

- AI 问数为什么不能只看 Demo
- Data Agent 上线前要怎么做验证
- 数据团队应该怎么设计 Skills / MCP / CLI 工作流
- AI 生成 SQL 为什么需要 Review 和权限卡点
- 数仓工程师在 AI 时代如何升级自己的能力

You can find me as:

- 抖音 / B站 / 小红书：`Seven聊数仓AI`
- 微信：`SevenDataAI`

## Principles

我更关心能不能落地，而不是概念是否好听。

AI 数据工程里最重要的不是“模型会不会回答”，而是：

- 口径能不能对齐
- SQL 能不能审查
- 权限能不能拦截
- 结果能不能追溯
- 错误能不能归因
- 改动后能不能回归

如果这些问题解决不了，AI 问数永远只能停在 Demo。
