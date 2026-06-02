# 项目级技能目录规范

本目录用于存放仓库级 AI 技能。

## 目录规则

- 固定根目录：`.agents/skills/`
- 每个技能独立目录：`.agents/skills/<skill-name>/`
- `<skill-name>` 仅允许：`[a-z0-9-]`

## 每个技能的最小文件集合

1. `SKILL.md`：技能说明（名称、用途、输入输出、依赖）
2. `install.sh`：安装脚本（幂等、失败即退出）
3. `use.md`：使用说明（触发条件、示例、故障排查）

## 推荐结构

```text
.agents/skills/
  <skill-name>/
    SKILL.md
    install.sh
    use.md
```
