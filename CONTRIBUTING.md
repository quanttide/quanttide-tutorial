# 量潮教程 — 贡献指南

## 目录结构

```
quanttide-tutorial/
├── intro/                    → 通识层：无前置，任何背景都能直接学
├── middle/                   → 中级层：需要一门专业前置（工程栈、方法论）
├── advanced/                 → 高级层：需要理论或架构级前置
├── default/company           → 主体层：法人主体教程
├── README.md                → 教程清单与项目定位
├── AGENTS.md                → Agent 工作指南
├── CHANGELOG.md             → 版本变更记录
└── CONTRIBUTING.md          → 本文件
```

目录按**学习顺序**排列：通识 → 中级 → 高级 → 主体。新增教程时按**前置门槛**定层；目录只有层，不设学科二级目录，学科分类在 README.md 教程清单中按学科分组承载（分组以 `quanttide-specification-of-disciplines` 为参照，不在本仓库自立学科）。

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
