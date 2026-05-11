# 设计方案：SecondMe 项目展示页

## 推荐方向

采用 `A + B + C` 融合方案：

- A：项目作品集型主页，适合对外展示和面试场景
- B：内部组织地图作为 Dashboard，方便 Vince 自己切换上下文
- C：宣言感融入首屏和开场文案，让页面更高级、更有思想密度

## 页面语言

- 默认使用中文。
- `SecondMe` 作为公司名，不翻译。
- `Dashboard` 可保留英文名称。
- Dashboard 部门名称使用中英文双语。

## 信息架构

顶部导航建议：

- `项目概览`
- `组织结构`
- `治理边界`
- `路线图`
- `Dashboard`

页面主体建议：

1. Hero 首屏
   - 标题：`SecondMe 不是一个聊天机器人，而是一家属于 Vince 的个人 AI 公司。`
   - 副标题说明 SecondMe 将身份、长期记忆、部门协作、权限治理和执行 harness 组织成可持续演化的个人工作系统。
   - 主按钮：查看项目
   - 次按钮：打开 Dashboard

2. 项目概览
   - 解释 SecondMe 是什么
   - 强调 Codex 是执行伙伴，SecondMe 拥有身份、记忆、组织和长期规则

3. 组织结构
   - 展示总经办和各部门
   - 强调任务先经过 Vincy / CEO Office 路由
   - 部门包括学习、知识、职业、工程、行为研究、运营、共享记忆、Agent Factory、Harness、产品战略

4. 治理边界
   - 展示 A0 / A1 / A2 权限模型
   - 让外部读者理解 SecondMe 不是无边界自动化，而是可解释、可确认、可追踪的协作系统

5. 路线图
   - 当前阶段：文档驱动的最小可用 AI 公司
   - 下一阶段：更强需求归档、展示页、Dashboard、工作流沉淀

6. Dashboard
   - 作为菜单中的内部视图，不抢主页叙事
   - 展示当前状态、部门地图、记忆与日志入口、近期迭代

## Dashboard 部门命名

建议使用：

- `总经办 CEO Office`
- `治理 Governance`
- `学习 Learning`
- `知识 Knowledge`
- `职业 Career`
- `工程 Engineering`
- `行为研究 Behavior Lab`
- `运营 Operations`
- `共享记忆 Shared Memory`
- `Agent 工厂 Agent Factory`
- `Harness 执行层`
- `产品战略 Product Strategy`

## 视觉方向

关键词：

- 高级
- 克制
- 清晰
- 作品集质感
- 组织系统感

建议风格：

- 浅色背景为主，搭配深色文字和少量强调色
- 使用细边框、柔和阴影和稳定网格
- 不使用廉价大渐变、过度装饰或一眼模板化的 hero
- 页面应该像一个成熟项目的 case study，而不是营销落地页

## 交互原则

- 单 HTML 页面内完成主要展示。
- 导航锚点滚动到对应 section。
- Dashboard 可以作为页面内 section，或通过菜单切换到 Dashboard 视图。
- 交互只服务浏览和理解，不做复杂状态管理。
