# 量潮教程 — ROADMAP

## 当前阶段

- [x] 仓库初始化（`data/` 下挂 3 个教程子模块）
- [x] 聚合容器重建：分层（通识/学科/主体）+ 学科分目录，70 个教程子仓库全量登记
- [x] 明确层序即学习顺序：`general` → `disciplines` → `default`，README/AGENTS/CONTRIBUTING 与 `.gitmodules` 一致按此排列
- [x] 取消领域层：`domains/` 的 33 个教程按学科并入 `disciplines/`，学科层扩到 10 个学科
- [ ] 各教程内容填充（在 `quanttide-tutorial-of-*` 子仓库内维护）
- [ ] 未接入教程的 14 个领域补齐 `docs/tutorial` 指针：`business`、`crowd`、`delib`、`design`、`docs`、`econ`、`entrep`、`health`、`innov`、`knowl`、`relation`、`sales`、`secret`、`security`
- [ ] 学科清单在 `quanttide-specification-of-disciplines` 落地，本仓库学科目录与之对齐
- [ ] 文档站构建与发布（MyST，可选）

## 预留项（暂不开发）

| # | 项 | 说明 |
|---|----|------|
| 1 | `quanttide-tutorial-of-product` | 云端空仓库，内容并入 `quanttide-tutorial-of-product-development` 后清理 |
| 2 | `quanttide-tutorial-of-software-architecture` | 云端空仓库，待定归属（计算机科学与技术） |
| 3 | 教程与课程的衔接 | 教程（怎么学会）与课程（怎么教出去）的边界与流水线 |
| 4 | 学科层细分 | 当前学科只到一级（如 `computer-science`），后续是否按二级学科再分待定 |
| 5 | 管理学与计算机科学与技术两科偏重 | 各 22 个，占学科层 2/3；后续可考虑按二级学科（工商管理/管理科学与工程等）再分 |

## 演进记录

- 2026-09-29：取消领域层。`domains/` 的 33 个教程按学科并入 `disciplines/`——学科层由 6 个学科扩到 10 个（新增教育学、新闻传播学、设计学、心理学），共 66 个教程；层序收敛为 `general`（通识）→ `disciplines`（学科）→ `default`（主体）。
- 2026-09-29：聚合容器重建。`data/` 扁平结构改为分层，层序即学习顺序；70 个教程子仓库全量登记，目录名取长名；补 README/AGENTS/CONTRIBUTING/ROADMAP/LICENSE。
