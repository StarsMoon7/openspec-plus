# OpenSpec Plus

集成多个 AI coding 代理工作流框架的子项目集合。

## 子项目

| 子模块 | 说明 | 原始仓库 |
|---|---|---|
| [modules/openspec](modules/openspec) | Spec-driven development (SDD) 规范框架 | [Fission-AI/OpenSpec](https://github.com/Fission-AI/OpenSpec) |
| [modules/agent-skills](modules/agent-skills) | 生产级工程技能库 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) |
| [modules/superpowers](modules/superpowers) | Agentic skills 框架与开发方法论 | [obra/superpowers](https://github.com/obra/superpowers) |

## 初始化

```bash
git clone --recurse-submodules https://github.com/StarsMoon7/openspec-plus.git
```

如果已克隆但未拉子模块：

```bash
git submodule update --init --recursive
```

## 同步上游更新

```bash
# 拉取所有子模块的上游更新并合并
git submodule foreach 'git fetch upstream && git merge upstream/main'

# 提交子模块版本变更
git add modules/
git commit -m "sync: update submodules to upstream"
git push
```

## 目录结构

```
openspec-plus/
├── modules/
│   ├── openspec/        # SDD 规范框架
│   ├── agent-skills/    # 工程技能库
│   └── superpowers/     # 开发方法论
└── README.md
```
