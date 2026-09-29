# 量潮教程（quanttide-tutorial）

量潮教程体系的**聚合容器**——按层聚合各教程子仓库（Git 子模块）。各教程是独立仓库，独立演进，本仓库只追踪引用。

## 仓库定位

量潮教程（quanttide-tutorial）是量潮知识管理体系中的**教程聚合容器**。教程横跨**主体轴（Who it is）与领域轴（What it expresses）**，并向外延伸到量潮之外的学科体系，回答"知识怎么教出去、怎么学会"。

同一个领域的知识会以多种形态沉淀，各有分工：

| 类型 | 回答的问题 | 聚合容器 |
|:--|:--|:--|
| 章程 | 依据什么运行 | `assets/quanttide-bylaw` |
| 规范 | 按什么标准做 | `assets/quanttide-specification` |
| 手册 | 具体怎么做 | `assets/quanttide-handbook` |
| **教程** | **怎么学会** | `assets/quanttide-tutorial`（本仓库） |
| 档案 | 做过什么、成果如何 | `assets/quanttide-profile` |
| 日志 | 什么时候发生了什么 | `assets/quanttide-journal` |

## 分层与学习顺序

四个层，层名即目录名。层序即**学习顺序**：

```text
general 通识  →  disciplines 学科  →  domains 领域  →  default 主体
  共同基础         专业训练            量潮业务          主体惯例
```

先通识打底，再学科筑基，然后进入量潮领域，最后落到具体主体"我们这里怎么做"。越靠前的层越通用、越不依赖量潮；越靠后的层越专用、越贴近具体主体。

| 序 | 层 | 目录 | 判定标准 | 数量 |
|:--|:--|:--|:--|--:|
| 1 | 通识层 | `general/` | 跨学科的共同基础，不属于任何单一学科 | 3 |
| 2 | 学科层 | `disciplines/` | 主题 = 外部学科训练，目录名取学科长名 | 33 |
| 3 | 领域层 | `domains/` | 主题 = 某个量潮领域的业务本身，与 `domains/quanttide-*` 同源 | 33 |
| 4 | 主体层 | `default/` | 法人主体自己的工作教程 | 1 |

三条原则：

- **教程随领域走**：教程产出于所属领域，领域仓库通过 `docs/tutorial` 引用同一份教程子仓库——本仓库是这些引用的**聚合视图**，不是副本。
- **学科清单由标准定**：`disciplines/` 的学科划分以 `quanttide-specification-of-disciplines`（量潮学科分类标准）为准，本仓库只引用，不自立学科。
- **只聚合，不承载**：本仓库不存放教程内容。一处维护，多入口访问；子模块独立提交推送，本仓库只更新引用指针。

## 教程清单

按学习顺序排列。

### 通识层（3）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-markdown`](general/markdown) | 量潮Markdown教程 |
| [`quanttide-tutorial-of-readme`](general/readme) | 量潮基础教程 |
| [`quanttide-tutorial-of-writing`](general/writing) | 量潮写作教程 |

### 学科层（33）

| 学科 | 教程 | 定位 |
|:--|:--|:--|
| 计算机科学与技术 | [`quanttide-tutorial-of-aigc-source-code`](disciplines/computer-science/aigc-source-code) | 量潮AIGC源码分析教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-big-data`](disciplines/computer-science/big-data) | 量潮大数据教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-building-cloud-services`](disciplines/computer-science/building-cloud-services) | 量潮云服务研发教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-cloud-computing`](disciplines/computer-science/cloud-computing) | 量潮云计算教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-computer-fundamentals`](disciplines/computer-science/computer-fundamentals) | 量潮计算机基础教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-data-analytics`](disciplines/computer-science/data-analytics) | 量潮数据分析教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-deep-learning`](disciplines/computer-science/deep-learning) | 量潮深度学习教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-fastapi`](disciplines/computer-science/fastapi) | 量潮FastAPI教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-flutter`](disciplines/computer-science/flutter) | 量潮Flutter教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-generative-ai`](disciplines/computer-science/generative-ai) | 量潮生成式人工智能教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-introduction-to-computer-systems`](disciplines/computer-science/introduction-to-computer-systems) | 量潮计算机系统结构教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-machine-learning`](disciplines/computer-science/machine-learning) | 量潮机器学习教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-microservices`](disciplines/computer-science/microservices) | 量潮微服务教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-operating-systems`](disciplines/computer-science/operating-systems) | 量潮操作系统教程 |
| 计算机科学与技术 | [`quanttide-tutorial-of-python`](disciplines/computer-science/python) | 量潮Python教程 |
| 经济学 | [`quanttide-tutorial-of-contract-theory`](disciplines/economics/contract-theory) | 量潮合约理论教程 |
| 经济学 | [`quanttide-tutorial-of-digital-economics`](disciplines/economics/digital-economics) | 量潮数字经济学教程 |
| 经济学 | [`quanttide-tutorial-of-econometrics`](disciplines/economics/econometrics) | 量潮计量经济学教程 |
| 经济学 | [`quanttide-tutorial-of-financial-economics`](disciplines/economics/financial-economics) | 量潮金融经济学教程 |
| 经济学 | [`quanttide-tutorial-of-industrial-organization`](disciplines/economics/industrial-organization) | 量潮产业组织教程 |
| 经济学 | [`quanttide-tutorial-of-macroeconomics`](disciplines/economics/macroeconomics) | 量潮宏观经济学教程 |
| 经济学 | [`quanttide-tutorial-of-microeconomics`](disciplines/economics/microeconomics) | 量潮微观经济学教程 |
| 经济学 | [`quanttide-tutorial-of-monetary-economics`](disciplines/economics/monetary-economics) | 量潮货币经济学教程 |
| 经济学 | [`quanttide-tutorial-of-public-economics`](disciplines/economics/public-economics) | 量潮公共经济学教程 |
| 经济学 | [`quanttide-tutorial-of-quantitative-trading`](disciplines/economics/quantitative-trading) | 量潮量化交易教程 |
| 经济学 | [`quanttide-tutorial-of-token-economics`](disciplines/economics/token-economics) | 量潮代币经济学教程 |
| 管理学 | [`quanttide-tutorial-of-financial-accounting`](disciplines/management/financial-accounting) | 量潮财务会计教程 |
| 管理学 | [`quanttide-tutorial-of-management`](disciplines/management/management) | 量潮管理学教程 |
| 管理学 | [`quanttide-tutorial-of-open-source`](disciplines/management/open-source) | 量潮开源管理教程 |
| 数学 | [`quanttide-tutorial-of-fourier-analysis`](disciplines/mathematics/fourier-analysis) | 量潮傅里叶分析教程 |
| 数学 | [`quanttide-tutorial-of-introduction-to-calculus`](disciplines/mathematics/introduction-to-calculus) | 量潮微积分教程（量潮高等数学教程） |
| 哲学 | [`quanttide-tutorial-of-philosophy`](disciplines/philosophy/philosophy) | 量潮哲学教程 |
| 社会学 | [`quanttide-tutorial-of-social-work`](disciplines/sociology/social-work) | 量潮社会工作教程 |

### 领域层（33）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-academic-research`](domains/academic-research) | 量潮学术研究教程 |
| [`quanttide-tutorial-of-agent-engineering`](domains/agent-engineering) | 量潮智能体工程教程 |
| [`quanttide-tutorial-of-asset-management`](domains/asset-management) | 量潮数字资产管理教程 |
| [`quanttide-tutorial-of-authorization-engineering`](domains/authorization-engineering) | 量潮身份认证教程 |
| [`quanttide-tutorial-of-cognitive-engineering`](domains/cognitive-engineering) | 量潮认知工程教程 |
| [`quanttide-tutorial-of-collaboration`](domains/collaboration) | 量潮团队协作教程 |
| [`quanttide-tutorial-of-communication-management`](domains/communication-management) | 量潮沟通管理教程 |
| [`quanttide-tutorial-of-course-development`](domains/course-development) | 量潮课程研发教程 |
| [`quanttide-tutorial-of-customer-relations`](domains/customer-relations) | 量潮客户关系教程 |
| [`quanttide-tutorial-of-customer-support`](domains/customer-support) | 量潮客户支持教程 |
| [`quanttide-tutorial-of-data-engineering`](domains/data-engineering) | 量潮数据工程教程 |
| [`quanttide-tutorial-of-devops`](domains/devops) | 量潮DevOps教程 |
| [`quanttide-tutorial-of-entrepreneurial-management`](domains/entrepreneurial-management) | 量潮创业管理教程 |
| [`quanttide-tutorial-of-execution-management`](domains/execution-management) | 量潮执行管理教程 |
| [`quanttide-tutorial-of-finance-management`](domains/finance-management) | 量潮财务管理教程 |
| [`quanttide-tutorial-of-founding-cloud-providers`](domains/founding-cloud-providers) | 量潮云厂商创业教程 |
| [`quanttide-tutorial-of-growth-management`](domains/growth-management) | 量潮增长管理教程 |
| [`quanttide-tutorial-of-human-resources`](domains/human-resources) | 量潮人力资源教程 |
| [`quanttide-tutorial-of-interaction-design`](domains/interaction-design) | 量潮交互设计教程 |
| [`quanttide-tutorial-of-knowledge-engineering`](domains/knowledge-engineering) | 量潮知识工程教程 |
| [`quanttide-tutorial-of-knowledge-work`](domains/knowledge-work) | 量潮知识工作教程 |
| [`quanttide-tutorial-of-learning-management`](domains/learning-management) | 量潮学习管理教程 |
| [`quanttide-tutorial-of-narrative-engineering`](domains/narrative-engineering) | 量潮叙事工程教程 |
| [`quanttide-tutorial-of-organization-management`](domains/organization-management) | 量潮组织管理教程 |
| [`quanttide-tutorial-of-payment-engineering`](domains/payment-engineering) | 量潮支付工程教程 |
| [`quanttide-tutorial-of-product-design`](domains/product-design) | 量潮产品策划教程 |
| [`quanttide-tutorial-of-product-development`](domains/product-development) | 量潮产品研发教程 |
| [`quanttide-tutorial-of-product-operations`](domains/product-operations) | 量潮产品运营教程 |
| [`quanttide-tutorial-of-project-management`](domains/project-management) | 量潮项目管理教程 |
| [`quanttide-tutorial-of-social-media`](domains/social-media) | 量潮新媒体运营教程 |
| [`quanttide-tutorial-of-software-engineering`](domains/software-engineering) | 量潮软件工程教程 |
| [`quanttide-tutorial-of-strategy-management`](domains/strategy-management) | 量潮战略管理教程 |
| [`quanttide-tutorial-of-vibe-coding`](domains/vibe-coding) | 量潮氛围编程教程 |

### 主体层（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-business-entity`](default/company) | 量潮科技工作教程 |

## 目录结构

```text
quanttide-tutorial/
├── general/               # 通识层：markdown、readme、writing
├── disciplines/           # 学科层：按学科分目录
│   ├── computer-science/  # 计算机科学与技术（15）
│   ├── economics/         # 经济学（11）
│   ├── management/        # 管理学（3）
│   ├── mathematics/       # 数学（2）
│   ├── philosophy/        # 哲学（1）
│   └── sociology/         # 社会学（1）
├── domains/               # 领域层：33 个领域教程（见上表）
├── default/               # 主体层：company
├── AGENTS.md              # 智能体约定
├── CHANGELOG.md           # 版本变更记录
├── CONTRIBUTING.md        # 贡献指南
├── LICENSE                # Apache-2.0 许可证
├── README.md              # 本文件
└── ROADMAP.md             # 路线图
```

## 快速开始

```bash
# 克隆（含子模块）
git clone --recurse-submodules https://github.com/quanttide/quanttide-tutorial.git

# 已有克隆时初始化/更新子模块
git submodule update --init --recursive
```

子模块是独立仓库，改动请在各教程仓库内提交推送，本仓库只更新引用；日常同步与提交约定见 [CONTRIBUTING.md](CONTRIBUTING.md)，智能体约定见 [AGENTS.md](AGENTS.md)。

## 关联

- 同源聚合容器：`assets/quanttide-bylaw`（章程）、`assets/quanttide-specification`（规范）、`assets/quanttide-handbook`（手册）、`assets/quanttide-profile`（档案）、`assets/quanttide-journal`（日志）
- 领域仓库：`domains/quanttide-*`，各领域通过 `docs/tutorial` 引用对应教程
- 学科标准：`quanttide-specification-of-disciplines`（量潮学科分类标准）
- 主仓库：[quanttide](https://github.com/quanttide/quanttide)

## 许可证

本项目采用 [Apache-2.0](LICENSE) 许可证。
