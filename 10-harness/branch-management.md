# 分支管理机制

## 目标

分支管理用于区分 SecondMe 中已经确认的规则、正在试运行的草案，以及用于 AB 测试的候选方案。

## 核心分支

### `master`

`master` 保存 Vince 已确认并启用的 SecondMe 内容。

适合进入 `master` 的内容：

- 已确认的画像偏好和稳定事实
- 已启用的工作流、留痕机制和低风险自动化
- 已确认的部门职责、agent 岗位说明和 SOP
- 已完成并通过检查的运行日志、变更记录和决策记录

每日复盘中 A 档低风险更新可以直接进入 `master`，但必须可追踪、可回滚，并在日志中留痕。

### `pre-release`

`pre-release` 保存待确认内容、候选机制和试运行草案。

适合进入 `pre-release` 的内容：

- 需要 Vince 确认的 agent 提示词草案
- 重要文档或 SOP 的候选修改
- Vincy 表达风格、日报格式、流程口径的候选版本
- 需要观察效果后再决定是否进入 `master` 的优化

`pre-release` 中的内容不得被当作已确认事实。进入 `master` 前需要在日报或决策日志中记录确认依据。

### `codex/*`

`codex/*` 分支用于短期开发、实验和 AB 测试。

适合使用 `codex/*` 的场景：

- 一次性实现某个明确任务
- 同时比较两个以上候选方案
- 在进入 `pre-release` 前做临时验证

完成后应明确结果：合并到 `master`、合并到 `pre-release`、继续观察，或废弃。

## 自动管理规则

每日复盘任务应按以下规则处理分支：

1. 已确认且低风险的记录更新，提交到 `master`。
2. 待确认但值得保留的草案，提交到 `pre-release`。
3. 存在两种以上候选方案时，创建 `codex/ab-<topic>-<variant>` 分支，并在日报中说明差异。
4. 不确定风险等级时，按更高风险处理，先放入 `pre-release` 或只报告不提交。
5. 每次自动提交都应在 `logs/run-log.md` 或 `logs/change-log.md` 留痕。

## 晋级流程

`pre-release` 内容进入 `master` 前，应满足以下条件：

- Vince 已确认采用该内容
- 已说明变更原因和影响范围
- 已检查不会绕过 `00-governance/permission-boundaries.md`
- 必要时已记录到 `logs/decision-log.md`

确认后可以通过 merge 或 cherry-pick 进入 `master`。
