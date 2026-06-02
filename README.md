# github-claw

个人 AI 工作空间，通过 GitHub Copilot 网页版长期使用。

## 快速入口

| 文件 | 用途 |
|------|------|
| [`AGENTS.md`](./AGENTS.md) | 助手角色定义、工作规则、记忆管理（**每次对话必读**） |
| [`memory/LONG_TERM.md`](./memory/LONG_TERM.md) | 长期事实：用户偏好、项目背景、重要决策 |
| [`memory/LOG.md`](./memory/LOG.md) | 时序任务日志 |

## 目录结构

```
.
├── AGENTS.md          # 核心：角色与规则
├── memory/
│   ├── LONG_TERM.md   # 长期记忆
│   └── LOG.md         # 任务日志
├── projects/          # 具体项目（按需创建）
└── tools/             # 工具脚本（按需创建）
```

> 这个仓库由 AI 助手 **Claw** 持续维护。每次新对话开始时，请先阅读 `AGENTS.md`。