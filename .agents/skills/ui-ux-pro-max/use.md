# ui-ux-pro-max 使用说明

## 何时调用
当用户要求为某个项目创建"高颜值官网"、"导航页"、"落地页"，或明确要求使用 UI-UX-PRO-MAX 技能时。

## 前置条件
- 已知产品名称、核心特性、用户场景
- 目标仓库存在 `docs/` 目录（没有则创建）
- GitHub 仓库已开启或将开启 GitHub Pages（源：`docs/` 目录或 Actions）

## 调用流程

1. 收集产品信息（名称、Slogan、特性、场景）
2. 在 `docs/index.html` 生成完整单文件落地页
3. 确保页面包含以下区块：
   - Hero（标题 + Slogan + CTA 按钮）
   - 核心特性（图标卡片）
   - 使用流程（How it works）
   - 用户场景（对比表格或卡片）
   - Footer（项目链接）
4. 配置 GitHub Pages 部署（Actions workflow 或 Settings）
5. 给出最终可访问 URL

## 最小示例

```
输入：产品名"扫码即传"，特性：零安装、实时同步、局域网传输
输出：docs/index.html（可访问地址 https://<user>.github.io/<repo>/）
```

## 常见失败与排查

| 问题 | 原因 | 解决 |
|------|------|------|
| 页面 404 | GitHub Pages 未启用 | 在 Settings > Pages 中启用，源选 `docs/` 或 `GitHub Actions` |
| 样式错乱 | 浏览器兼容性 | 使用 CSS 变量 + Flex/Grid，避免实验性特性 |
| 中文乱码 | 缺少 charset | 确保 `<meta charset="UTF-8">` 在 `<head>` 首行 |
