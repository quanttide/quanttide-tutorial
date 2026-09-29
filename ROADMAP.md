# 量潮教程 — ROADMAP

## 当前阶段

- [x] 仓库初始化（`data/` 下挂 3 个教程子模块）
- [x] 聚合容器重建：分层（主体/领域/学科/通识）+ 学科分目录，70 个教程子仓库全量登记
- [ ] 各教程内容填充（在 `quanttide-tutorial-of-*` 子仓库内维护）
- [ ] 未接入教程的 14 个领域补齐 `docs/tutorial` 指针：`business`、`crowd`、`delib`、`design`、`docs`、`econ`、`entrep`、`health`、`innov`、`knowl`、`relation`、`sales`、`secret`、`security`
- [ ] 学科清单在 `quanttide-specification-of-disciplines` 落地，本仓库学科目录与之对齐
- [ ] 文档站构建与发布（MyST，可选）

## 预留项（暂不开发）

| # | 项 | 说明 |
|---|----|------|
| 1 | `quanttide-tutorial-of-product` | 云端空仓库，内容并入 `quanttide-tutorial-of-product-development` 后清理 |
| 2 | `quanttide-tutorial-of-software-architecture` | 云端空仓库，待定归属（`code` 领域） |
| 3 | 教程与课程的衔接 | 教程（怎么学会）与课程（怎么教出去）的边界与流水线 |
| 4 | 学科层细分 | 当前学科只到一级（如 `computer-science`），后续是否按二级学科再分待定 |

## 演进记录

- 2026-09-29：聚合容器重建。`data/` 扁平结构改为四层——`default/`（主体）+ `domains/`（领域）+ `disciplines/`（学科，按学科分目录）+ `general/`（通识）；70 个教程子仓库全量登记，目录名取长名；补 README/AGENTS/CONTRIBUTING/ROADMAP/LICENSE。
