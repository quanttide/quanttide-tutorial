# AGENTS.md - Agent 工作指南

本文档为 Agent（包括 CodeBuddy、Claude Code、Cursor、GitHub Copilot 等）在本仓库中工作提供指南。

## 核心记忆

### 项目定位

量潮教程（quanttide-tutorial）是量潮知识管理体系中教程的**聚合容器**（主体轴/Who it is + 领域轴/What it expresses），采用 Git 子模块架构聚合各法人主体与领域的教程仓库。

### 子模块管理

- 子模块独立维护，本仓库只追踪引用指针
- **禁止**：直接在父仓库修改子模块文件
- **必须**：在子模块仓库独立提交推送，父仓库只更新引用
- **新增子模块**：按层落位，并同步更新 README.md 教程清单与 CHANGELOG.md
- **目录命名**：目录名一律取教程仓库名去掉 `quanttide-tutorial-of-` 前缀（域长名 / 学科长名 / 教程长名），如 `quanttide-tutorial-of-data-engineering` → `domains/data-engineering`

### 分层

层序即**学习顺序**：`general`（通识）→ `disciplines`（学科）→ `domains`（领域）→ `default`（主体）。

| 序 | 层 | 目录 | 落位判定 |
|:--|:--|:--|:--|
| 1 | 通识层 | `general/<教程长名>` | 跨学科的共同基础，不属于任何单一学科 |
| 2 | 学科层 | `disciplines/<学科>/<教程长名>` | 主题 = 外部学科训练；学科名以 `quanttide-specification-of-disciplines` 为准 |
| 3 | 领域层 | `domains/<域长名>` | 主题 = 某个量潮领域的业务本身，与 `domains/quanttide-*` 同源 |
| 4 | 主体层 | `default/company` | 法人主体自己的工作教程 |

## 人机协作范式

1. **最小干预**：仅在用户明确请求时操作
2. **信息复用**：优先使用已有文档内容
3. **维护记录**：修改后同步更新 CHANGELOG.md
4. **原子提交**：每次提交包含完整独立变更
5. **提交即推送**：提交后默认推送到远端，除非用户明确说"只提交不推"

## 必查文档清单

| 任务类型 | 必查文档 | 查阅内容 |
|----------|----------|----------|
| 修改文档/添加内容 | README.md | 教程清单、结构树、分类边界 |
| 提交代码 | CHANGELOG.md | 版本记录格式、最新版本 |
| 更新子模块 | .gitmodules | 子模块注册状态 |
| 新增/移除教程 | README.md + CHANGELOG.md | 清单同步、变更记录 |
