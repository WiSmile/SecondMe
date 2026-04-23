# 10 Harness

Harness 是 SecondMe 的执行层，负责调度、日志、权限、工具调用和评估。

第一阶段只定义模块边界，不急于实现复杂自动化。

## 第一版模块

- `dispatcher`：任务接收、拆解、分发
- `memory`：长期记忆、短期上下文、共享记忆管理
- `policy`：权限规则、审批规则、风险边界
- `tooling`：Codex、脚本、文件系统、电脑操作等工具接入
- `evaluation`：任务复盘、效果评估、agent 规则迭代建议

