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

四个层，层名即目录名。层序即**学习顺序**，按**前置门槛**分层：

```text
intro 通识  →  middle 中级  →  advanced 高级  →  default 主体
  无前置          一门前置         理论/架构前置       主体惯例
```

先通识打底，再逐级深入，最后落到具体主体"我们这里怎么做"。越靠前的层越通用、越不依赖量潮；越靠后的层越专用、越贴近具体主体。

| 序 | 层 | 目录 | 判定标准 | 数量 |
|:--|:--|:--|:--|--:|
| 1 | 通识层 | `intro/` | 不需要专业前置，任何背景都能直接学 | 4 |
| 2 | 中级层 | `middle/` | 需要一门专业前置（工程栈、方法论） | 58 |
| 3 | 高级层 | `advanced/` | 需要理论或架构级前置 | 11 |
| 4 | 主体层 | `default/` | 法人主体自己的工作教程 | 1 |

三条原则：

- **目录只有层，不设学科目录**：学科分类由本页教程清单承载（按学科分组呈现），不落成目录。
- **教程随领域走**：教程产出于所属领域，领域仓库通过 `docs/tutorial` 引用同一份教程子仓库——本仓库是这些引用的**聚合视图**，按难度分层呈现。
- **只聚合，不承载**：本仓库不存放教程内容。一处维护，多入口访问；子模块独立提交推送，本仓库只更新引用指针。

## 教程清单

按学习顺序排列。中级与高级层内按学科分组；学科划分以 `quanttide-specification-of-disciplines`（量潮学科分类标准）为参照，本仓库只引用，不自立学科。

### 通识层 intro（4）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-markdown`](intro/markdown) | 量潮Markdown教程 |
| [`quanttide-tutorial-of-writing`](intro/writing) | 量潮写作教程 |
| [`quanttide-tutorial-of-readme`](intro/readme) | 量潮基础教程 |
| [`quanttide-tutorial-of-vibe-coding`](intro/vibe-coding) | 量潮氛围编程教程 |

### 中级层 middle（58）

共 58 个。按学科分组（学科不落目录，分类在此承载）：

#### 计算机科学与技术（17）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-devops`](middle/devops) | 量潮DevOps教程 |
| [`quanttide-tutorial-of-fastapi`](middle/fastapi) | 量潮FastAPI教程 |
| [`quanttide-tutorial-of-flutter`](middle/flutter) | 量潮Flutter教程 |
| [`quanttide-tutorial-of-python`](middle/python) | 量潮Python教程 |
| [`quanttide-tutorial-of-building-cloud-services`](middle/building-cloud-services) | 量潮云服务研发教程 |
| [`quanttide-tutorial-of-cloud-computing`](middle/cloud-computing) | 量潮云计算教程 |
| [`quanttide-tutorial-of-big-data`](middle/big-data) | 量潮大数据教程 |
| [`quanttide-tutorial-of-microservices`](middle/microservices) | 量潮微服务教程 |
| [`quanttide-tutorial-of-operating-systems`](middle/operating-systems) | 量潮操作系统教程 |
| [`quanttide-tutorial-of-data-analytics`](middle/data-analytics) | 量潮数据分析教程 |
| [`quanttide-tutorial-of-agent-engineering`](middle/agent-engineering) | 量潮智能体工程教程 |
| [`quanttide-tutorial-of-generative-ai`](middle/generative-ai) | 量潮生成式人工智能教程 |
| [`quanttide-tutorial-of-knowledge-engineering`](middle/knowledge-engineering) | 量潮知识工程教程 |
| [`quanttide-tutorial-of-computer-fundamentals`](middle/computer-fundamentals) | 量潮计算机基础教程 |
| [`quanttide-tutorial-of-introduction-to-computer-systems`](middle/introduction-to-computer-systems) | 量潮计算机系统结构教程 |
| [`quanttide-tutorial-of-authorization-engineering`](middle/authorization-engineering) | 量潮身份认证教程 |
| [`quanttide-tutorial-of-software-engineering`](middle/software-engineering) | 量潮软件工程教程 |

#### 设计学（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-interaction-design`](middle/interaction-design) | 量潮交互设计教程 |

#### 经济学（7）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-industrial-organization`](middle/industrial-organization) | 量潮产业组织教程 |
| [`quanttide-tutorial-of-public-economics`](middle/public-economics) | 量潮公共经济学教程 |
| [`quanttide-tutorial-of-macroeconomics`](middle/macroeconomics) | 量潮宏观经济学教程 |
| [`quanttide-tutorial-of-microeconomics`](middle/microeconomics) | 量潮微观经济学教程 |
| [`quanttide-tutorial-of-payment-engineering`](middle/payment-engineering) | 量潮支付工程教程 |
| [`quanttide-tutorial-of-digital-economics`](middle/digital-economics) | 量潮数字经济学教程 |
| [`quanttide-tutorial-of-monetary-economics`](middle/monetary-economics) | 量潮货币经济学教程 |

#### 教育学（2）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-learning-management`](middle/learning-management) | 量潮学习管理教程 |
| [`quanttide-tutorial-of-course-development`](middle/course-development) | 量潮课程研发教程 |

#### 新闻传播学（2）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-narrative-engineering`](middle/narrative-engineering) | 量潮叙事工程教程 |
| [`quanttide-tutorial-of-social-media`](middle/social-media) | 量潮新媒体运营教程 |

#### 管理学（25）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-founding-cloud-providers`](middle/founding-cloud-providers) | 量潮云厂商创业教程 |
| [`quanttide-tutorial-of-product-development`](middle/product-development) | 量潮产品研发教程 |
| [`quanttide-tutorial-of-product-design`](middle/product-design) | 量潮产品策划教程 |
| [`quanttide-tutorial-of-product-operations`](middle/product-operations) | 量潮产品运营教程 |
| [`quanttide-tutorial-of-human-resources`](middle/human-resources) | 量潮人力资源教程 |
| [`quanttide-tutorial-of-entrepreneurial-management`](middle/entrepreneurial-management) | 量潮创业管理教程 |
| [`quanttide-tutorial-of-business-development`](middle/business-development) | 量潮商务拓展教程 |
| [`quanttide-tutorial-of-collaboration`](middle/collaboration) | 量潮团队协作教程 |
| [`quanttide-tutorial-of-growth-management`](middle/growth-management) | 量潮增长管理教程 |
| [`quanttide-tutorial-of-academic-research`](middle/academic-research) | 量潮学术研究教程 |
| [`quanttide-tutorial-of-customer-relations`](middle/customer-relations) | 量潮客户关系教程 |
| [`quanttide-tutorial-of-customer-support`](middle/customer-support) | 量潮客户支持教程 |
| [`quanttide-tutorial-of-open-source`](middle/open-source) | 量潮开源管理教程 |
| [`quanttide-tutorial-of-strategy-management`](middle/strategy-management) | 量潮战略管理教程 |
| [`quanttide-tutorial-of-execution-management`](middle/execution-management) | 量潮执行管理教程 |
| [`quanttide-tutorial-of-asset-management`](middle/asset-management) | 量潮数字资产管理教程 |
| [`quanttide-tutorial-of-communication-management`](middle/communication-management) | 量潮沟通管理教程 |
| [`quanttide-tutorial-of-knowledge-work`](middle/knowledge-work) | 量潮知识工作教程 |
| [`quanttide-tutorial-of-management`](middle/management) | 量潮管理学教程 |
| [`quanttide-tutorial-of-organization-management`](middle/organization-management) | 量潮组织管理教程 |
| [`quanttide-tutorial-of-market-management`](middle/market-management) | 量潮营销管理教程 |
| [`quanttide-tutorial-of-deliberation-management`](middle/deliberation-management) | 量潮议事管理教程 |
| [`quanttide-tutorial-of-financial-accounting`](middle/financial-accounting) | 量潮财务会计教程 |
| [`quanttide-tutorial-of-finance-management`](middle/finance-management) | 量潮财务管理教程 |
| [`quanttide-tutorial-of-project-management`](middle/project-management) | 量潮项目管理教程 |

#### 数学（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-introduction-to-calculus`](middle/introduction-to-calculus) | 量潮微积分教程（量潮高等数学教程） |

#### 元工程（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-meta-engineering`](middle/meta-engineering) | 量潮元工程教程 |

#### 心理学（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-cognitive-engineering`](middle/cognitive-engineering) | 量潮认知工程教程 |

#### 社会学（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-social-work`](middle/social-work) | 量潮社会工作教程 |

### 高级层 advanced（11）

共 11 个。按学科分组（学科不落目录，分类在此承载）：

#### 计算机科学与技术（4）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-aigc-source-code`](advanced/aigc-source-code) | 量潮AIGC源码分析教程 |
| [`quanttide-tutorial-of-data-engineering`](advanced/data-engineering) | 量潮数据工程教程 |
| [`quanttide-tutorial-of-machine-learning`](advanced/machine-learning) | 量潮机器学习教程 |
| [`quanttide-tutorial-of-deep-learning`](advanced/deep-learning) | 量潮深度学习教程 |

#### 经济学（5）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-token-economics`](advanced/token-economics) | 量潮代币经济学教程 |
| [`quanttide-tutorial-of-contract-theory`](advanced/contract-theory) | 量潮合约理论教程 |
| [`quanttide-tutorial-of-econometrics`](advanced/econometrics) | 量潮计量经济学教程 |
| [`quanttide-tutorial-of-quantitative-trading`](advanced/quantitative-trading) | 量潮量化交易教程 |
| [`quanttide-tutorial-of-financial-economics`](advanced/financial-economics) | 量潮金融经济学教程 |

#### 数学（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-fourier-analysis`](advanced/fourier-analysis) | 量潮傅里叶分析教程 |

#### 军事学（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-war-gaming`](advanced/war-gaming) | 量潮兵旗推演教程 |

### 主体层 default（1）

| 教程 | 定位 |
|:--|:--|
| [`quanttide-tutorial-of-business-entity`](default/company) | 量潮科技工作教程 |

## 目录结构

```text
quanttide-tutorial/
├── intro/                      # 通识层：4 个教程
├── middle/                     # 中级层：58 个教程（学科分类见教程清单）
├── advanced/                   # 高级层：11 个教程（学科分类见教程清单）
├── default/                    # 主体层：company
├── AGENTS.md                   # 智能体约定
├── CHANGELOG.md                # 版本变更记录
├── CONTRIBUTING.md             # 贡献指南
├── LICENSE                     # Apache-2.0 许可证
└── README.md                   # 本文件
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
