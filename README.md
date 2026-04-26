# SecondMe

SecondMe 是我的个人 AI 公司。

它不是单一工具，而是一个长期陪伴我的组织系统：通过部门、员工 agent、记忆、治理和 harness 执行层，持续辅助我学习、知识沉淀、求职成长、开发协作和电脑操作。

## 当前版本定位

第一版采用“文档驱动的最小可用 AI 公司”：

- 先建立组织结构、权限边界、部门职责和 agent 岗位说明书
- 优先服务我的学习沉淀、求职材料优化和个人画像积累
- 暂不追求复杂自动化，所有重要变更保持人工审批
- 为未来 harness、脚本、电脑操作能力预留清晰边界

## 使用入口

- 规范入口优先读取 `SECONDME_SPEC.md`
- 机器可读索引见 `secondme.spec.yaml`
- 新资料统一放入 `inbox/`
- 当前任务由 `01-ceo-office/` 统一接收和拆解
- 产品规划和迭代建议进入 `11-product-strategy/`
- 长期事实与画像沉淀到 `08-shared-memory/`
- 知识整理进入 `03-knowledge/`
- 求职相关进入 `04-career/`
- 决策、审批和变更记录写入 `logs/`

## 在 Codex 中使用 SecondMe

在 Codex 中称呼 `Vincy`，即可唤醒 SecondMe 工作方式。

示例：

- `Vincy，帮我整理这份学习笔记`
- `Vincy，按 SecondMe 流程分析这个岗位 JD`
- `Vincy，帮我判断这件事应该交给哪个部门`

唤醒后，Codex 默认以总经办 Chief of Staff Agent 的身份工作，先理解目标，再读取必要的治理、共享记忆和部门文档，最后协调对应部门完成任务。

相关入口：

- `SECONDME_SPEC.md`
- `secondme.spec.yaml`
- `AGENTS.md`
- `01-ceo-office/vincy-entrypoint.md`
- `10-harness/codex-adapter.md`

## 核心原则

1. SecondMe 是组织层，harness 是执行层。
2. 我主要对接总经办，其他部门尽量减少打扰。
3. 自动化从低风险的信息整理开始。
4. 写代码、改重要文档、更新 SOP 和 agent 提示词需要我确认。
5. 电脑操作、对外发送、删除重要内容、改权限和改核心身份设定必须我批准。
