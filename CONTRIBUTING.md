# 量潮教程 — 贡献指南

## 目录结构

```
quanttide-tutorial/
├── general/                 → 通识层：跨学科共同基础
├── disciplines/             → 学科层：学科教程 + 归属该学科的量潮领域教程
├── default/company          → 主体层：法人主体教程
├── README.md                → 教程清单与项目定位
├── AGENTS.md                → Agent 工作指南
├── ROADMAP.md               → 路线图
├── CHANGELOG.md             → 版本变更记录
└── CONTRIBUTING.md          → 本文件
```

目录按**学习顺序**排列：通识 → 学科 → 主体。新增教程时先定层：跨学科共同基础 → `general/`；其余一律按学科进 `disciplines/<学科>/`（量潮领域教程也不例外，领域知识本就是学科的分支）；法人主体自己的工作教程 → `default/company`。学科名以 `quanttide-specification-of-disciplines` 为准，不在本仓库自立学科。

## 内容规范

- 文档用中文
- 教程回答"怎么学会"，与规范（按什么标准做）、手册（具体怎么做）分工不重叠
- 教程内容在对应子仓库（`quanttide-tutorial-of-*`）内独立维护，本仓库不直接存放教程内容
- 同一份教程可能被领域仓库以 `docs/tutorial` 引用——只在一处维护，不要在父仓库复制副本

## 提交流程

1. 在子模块内提交推送（Conventional Commits）
2. 回到父仓库更新子模块指针，提交推送
3. 新增/移除教程时同步更新 README.md 教程清单与结构树
4. 变更记录写入 CHANGELOG.md
