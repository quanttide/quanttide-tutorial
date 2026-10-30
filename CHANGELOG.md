# CHANGELOG

所有显著变更都将记录在此文件中。

格式基于 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.0.0/)。

---

## [0.3.1] - 2026-10-30

### 变更

- 子模块改名：`middle/philosophy` → `middle/meta-engineering`（量潮元工程教程），目录与仓库名（`quanttide-tutorial-of-meta-engineering`）对齐；原哲学教程待需要时另行新建

## [Unreleased]

### 新增

- 新增子模块 `advanced/war-gaming`（量潮兵旗推演教程）：教程由 73 增至 74（高级层 10 → 11，军事学分组）
- `advanced/war-gaming` `intro/` 三部曲迁入：兵棋推演入门、用真实历史造一盘棋、反事实推演，自 `quanttide-tutorial-of-founder` 的 `war/` 分区迁出

## [0.3.0] - 2026-10-30

### 变更

- 分层重划：由「通识/学科/主体」三层改为按**前置门槛**的四层——`intro`（通识，无前置）→ `middle`（中级，一门前置）→ `advanced`（高级，理论/架构前置）→ `default`（主体）
- 取消学科二级目录：原 `disciplines/<学科>/` 拆平，68 个学科教程直接落层目录（`middle/` 58 个、`advanced/` 10 个）；`general/` 4 个教程并入 `intro/`
- 学科分类改由 README 教程清单承载（按学科分组呈现），不再落成目录
- 子模块移层：`disciplines/computer-science/vibe-coding`（氛围编程教程）迁入通识层，用词统一为「氛围编程」
- README、AGENTS.md、CONTRIBUTING.md 分层说明与结构树同步重写

## [0.2.0] - 2026-09-29

### 变更

- 聚合容器重建：`data/` 扁平结构改为分层，层序即学习顺序 `general`（通识）→ `disciplines`（学科）→ `default`（主体）
- 取消领域层：33 个量潮领域教程按学科并入 `disciplines/`，学科层由 6 个学科扩到 10 个（新增教育学、新闻传播学、设计学、心理学）
- 目录名统一取教程仓库名去掉 `quanttide-tutorial-of-` 前缀（学科长名 / 教程长名），如 `quanttide-tutorial-of-data-engineering` → `disciplines/computer-science/data-engineering`
- 原 `data/` 下 3 个子模块迁入 `disciplines/computer-science/`：`big-data`、`data-analytics`、`data-engineering`
- 教程清单全量登记：挂载 70 个教程子仓库（通识 3 + 学科 66 + 主体 1）
- 新增子模块 `disciplines/management/market-management`（营销管理教程）：从量潮科技工作教程迁出 `market/`，教程由 70 增至 71（学科 67）
- 新增子模块 `disciplines/management/business-development`（商务拓展教程）、`disciplines/management/deliberation-management`（议事管理教程）：教程由 71 增至 73（学科 69）
- 同步公司教程迁出：`agent-engineering`、`asset-management`、`communication-management`、`devops`、`finance-management`、`organization-management`、`open-source`、`social-media`、`strategy-management`、`narrative-engineering` 十个领域教程接收迁移内容，公司教程收敛为主体层（入门 + 六条业务线 + 附录）
- `.gitmodules`、README 清单与结构树、AGENTS 落位表、CONTRIBUTING 结构树一律按学习顺序排列
- README 重写：仓库定位、类型分工、分层与学习顺序、教程清单（按学科分组）、目录结构、快速开始

### 新增

- 新增分层文档：`AGENTS.md`（含分层落位判定）、`CONTRIBUTING.md`、`ROADMAP.md`
- 新增 `LICENSE`（Apache-2.0）

## [v0.1.0] - 2026-05-23

### Added
- 项目初始化
- 添加 qtdata 子模块（data/quanttide-tutorial-of-big-data）
- 添加 data analytics 子模块（data/quanttide-tutorial-of-data-analytics）
- 添加 data engineering 子模块（data/quanttide-tutorial-of-data-engineering）

### Changed
- 将 qtdata/ 目录重命名为 data/
