# 实现计划：SecondMe 项目展示页

## 推荐产物

创建一个可直接打开的静态 HTML 文件。

建议路径：

- `showcase/secondme-showcase.html`

如果后续需要更多资产，可扩展为：

- `showcase/index.html`
- `showcase/assets/`

## 步骤

1. 确认正式页面保存路径。
2. 从当前 SecondMe 文档中提炼页面内容：
   - `SECONDME_SPEC.md`
   - `README.md`
   - `00-governance/permission-boundaries.md`
   - `01-ceo-office/vincy-entrypoint.md`
   - `11-product-strategy/README.md`
3. 编写单文件 HTML：
   - 语义化结构
   - 内联 CSS
   - 少量导航交互
4. 实现响应式布局：
   - 桌面端展示完整网格和 Dashboard
   - 移动端改为单列，避免文字挤压
5. 浏览器验证：
   - 打开本地 HTML
   - 检查桌面端和移动端布局
   - 检查中文文案、部门双语命名和导航锚点
6. 根据 Vince 反馈微调视觉和文案。

## 验证重点

- 首屏是否足够高级、清晰、有项目辨识度
- 是否准确表达 SecondMe 的“个人 AI 公司”定位
- Dashboard 是否是菜单中的内部视图，而不是主页主叙事
- 文字是否在不同宽度下不重叠、不溢出
- 是否避免对 SecondMe 当前能力的过度承诺
