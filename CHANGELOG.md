# CHANGELOG

所有显著变更都将记录在此文件中。

格式基于 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.0.0/)。

---

## [Unreleased]

### 变更

- 聚合容器重建：`data/` 扁平结构改为四层，层序即学习顺序 `general`（通识）→ `disciplines`（学科，按学科分目录）→ `domains`（领域）→ `default`（主体）
- `.gitmodules`、README 清单与结构树、AGENTS 落位表、CONTRIBUTING 结构树一律按学习顺序排列
- 目录名统一取教程仓库名去掉 `quanttide-tutorial-of-` 前缀（长名），如 `quanttide-tutorial-of-data-engineering` → `domains/data-engineering`
- 原 `data/` 下 3 个子模块迁入新层：`big-data`、`data-analytics` → `disciplines/computer-science/`，`data-engineering` → `domains/`
- 教程清单全量登记：挂载 70 个教程子仓库（主体 1 + 领域 33 + 学科 33 + 通识 3）
- README 重写：仓库定位、类型分工、分层与落位判定、教程清单（分层列表）、目录结构、快速开始

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
