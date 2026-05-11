# SecondMe 路径注册表

> 用途：让 Vincy 在执行学习、知识沉淀、文件写入、项目整理任务时，先定位正确工作区，避免把 SecondMe 工作区和 Obsidian 知识库混淆。

## 核心路径

| 名称 | 路径 | 用途 |
|---|---|---|
| SecondMe 工作区 | `/Users/vince/code/SecondMe` | Vincy 的组织规则、流程、部门、治理文件、长期运行约定 |
| Obsidian 知识库 | `/Users/vince/Documents/Obsidian-SecondMe` | Vince 的正式知识库和学习笔记沉淀位置 |
| Obsidian 学习区 | `/Users/vince/Documents/Obsidian-SecondMe/学习` | 技术学习、课程、主题知识整理 |
| Obsidian Redis 学习区 | `/Users/vince/Documents/Obsidian-SecondMe/学习/Redis` | Redis 学习笔记、面试题、图解和复习材料 |
| Obsidian MySQL 学习区 | `/Users/vince/Documents/Obsidian-SecondMe/学习/MySQL` | MySQL 学习笔记、面试题、图解和复习材料 |

## 路径口径

当前 SecondMe 工作区的权威路径是 `/Users/vince/code/SecondMe`。

历史日志、早期设计文档或旧日报中如果出现 `/Users/vince/SecondMe`，应视为旧路径口径，仅用于理解历史记录，不作为新的读取或写入目标。

## 路径判断规则

当 Vince 提到以下表达时，默认目标是 Obsidian 知识库，而不是 SecondMe 工作区：

- “放到 Obsidian”
- “整理成学习文档”
- “沉淀成笔记”
- “放到学习下面”
- “学习-Redis”
- “学习/MySQL”
- “整理到我的笔记里”

当 Vince 提到以下表达时，默认目标是 SecondMe 工作区：

- “固化流程”
- “更新 SecondMe 规则”
- “建立 SOP”
- “优化 SecondMe 项目”
- “学习部流程”
- “治理规则”
- “路径注册表”

## 写入边界

SecondMe 工作区用于保存流程、规则和组织结构；Obsidian 知识库用于保存可复习、可阅读、可链接的学习内容。

如果一个任务同时涉及两者：

1. 先在 SecondMe 工作区读取流程和规则。
2. 再在 Obsidian 知识库定位目标目录或文件。
3. 写入前确认目标目录存在。
4. 如果目标目录不存在，停止并询问 Vince。
5. 如果目标文件已存在，先读取再合并，避免覆盖已有内容。

## 常用落点

| 内容类型 | 默认落点 |
|---|---|
| 技术原理学习笔记 | `/Users/vince/Documents/Obsidian-SecondMe/学习/{主题}` |
| Redis 学习文档 | `/Users/vince/Documents/Obsidian-SecondMe/学习/Redis` |
| MySQL 学习文档 | `/Users/vince/Documents/Obsidian-SecondMe/学习/MySQL` |
| 面试复习资料 | 优先按技术主题放入 `学习/{主题}`，综合面试资料可放入 Obsidian 的 `找工作` |
| SecondMe 运行规则 | `/Users/vince/code/SecondMe/00-governance` |
| SecondMe 操作流程 | `/Users/vince/code/SecondMe/07-operations` |

## Vincy 执行提醒

处理文件写入任务时，Vincy 必须先判断这是“知识沉淀”还是“SecondMe 规则固化”。

- 知识沉淀：优先写入 Obsidian 知识库。
- 规则固化：优先写入 SecondMe 工作区。
- 不确定：先读路径注册表，再向 Vince 简短确认。
