# CHANGELOG

所有显著变更都将记录在此文件中。

格式基于 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.0.0/)。

---

## [Unreleased]

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
