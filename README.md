# AI × Quantum · 半年学习计划

学习周期：6 个月 · 每周 15 小时 · 更新 2026-09-16

[半年安排](#六个月安排) · [每周节奏](#每周节奏) · [第一个月详细计划](#第一个月详细计划)

## 学习目标

通过 **6 套主资源与 5 个专题模块**，建立 AI、量子系统、检索推荐与智能体的知识框架。主线方法以能够解释机制、设计实验和评价结果为目标；交叉领域先建立任务地图，再围绕主项目深入。

## 六套主资源

| 主资源 | 核心知识 | 学习阶段 |
| :--- | :--- | :--- |
| [D2L](https://d2l.ai/) | ML/DL、泛化、反传、优化、表示、attention/Transformer | M01–M02 |
| [Watrous / IBM 量子系列](https://arxiv.org/abs/2507.11536) | 态、测量、纠缠、密度矩阵、信道、算法、QEC | M01–M03 |
| [Berkeley CS285](https://rail.eecs.berkeley.edu/deeprlcourse/) | PG/actor-critic、DQN、PPO/SAC、探索、model-based/offline RL | M02 基础准备；M03 核心方法；M06 后训练 |
| [MARL Book](https://www.marl-book.com/) | MDP、games、Dec-POMDP、CTDE、信用分配、MAPPO/QMIX | M02 第 2 章；M04 多智能体 |
| [Personalized Machine Learning](https://cseweb.ucsd.edu/~jmcauley/pml/) | 协同过滤、隐因子、隐式反馈、内容与序列推荐 | M05 |
| [Hugging Face Agents](https://huggingface.co/learn/agents-course/en/unit0/introduction) | 工具、规划、记忆、Agentic RAG、验证与评价 | M06 |

各课程开始时先梳理知识地图、先修与选读范围。教材和录像按主题对应；CS285 采用 2026 课件，2023 录像用于基础概念补充。

### 课程知识地图与选读范围

- **D2L：**数据与概率 → 回归/分类 → 泛化与正则化 → MLP/反传 → 优化 → CNN/RNN → attention/Transformer。主读第 3–5、11、12 章；第 2 章按需补数学，CNN/RNN 以机制概览为主。
- **Watrous：**单/多系统与测量 → 电路与纠缠协议 → 密度矩阵/信道/一般测量/状态距离 → oracle 与量子算法 → 编码、错误离散化、可纠正性与 stabilizer。按 Basics、General Formulation、Algorithms、QEC 四单元选读。
- **CS285：**MDP/value/control → PG/actor-critic → Q-learning → PPO/SAC → 探索、model-based/offline RL → LLM RL。先用 MARL Book 第 2 章掌握 DP/MC/TD、on/off-policy，再进入深度 RL。
- **MARL Book：**单智能体复习 → games/solution concepts → Dec-POMDP 与非平稳性 → CTDE 与信用分配 → MAPPO/QMIX → 环境与评价。M04 选第 3–6、9–10 章，第 11 章选择一个环境。
- **PML：**预测任务 → 协同过滤/隐因子/隐式反馈 → 内容与结构 → 时间与序列。主读第 4–5 章，第 6–7 章选读核心概念，结合检索与系统专题检查评价方法。
- **HF Agents：**工具/动作/观测 → 一个框架 → Agentic RAG → 规划、记忆与失败恢复 → 验证与评价。选 Unit 1、Unit 2 的一个框架、Unit 3 与 evaluation bonus；后训练结合 CS285。


## 六个月安排

每个学习月包含 4 个学习周，共 60 小时。主线 32h、量子/应用线 20h、前沿与复盘 8h；实践包含在对应学习线内。

| 月份 | 主线 · 32h | 量子 / 应用线 · 20h | 阶段目标 |
| :--- | :--- | :--- | :--- |
| M01 | ML 任务、数据划分、泛化、正则化、分类；MLP 与反传入门 | 单/多系统、测量、电路、Bell 态；密度矩阵入门 | 解释训练流程与两 qubit 电路，完成一个小验证 |
| M02 | D2L：优化、归一化、CNN/RNN 概览、attention/Transformer（20h）；MARL 第 2 章与 CS285：MDP/value、DP/MC/TD、on/off-policy（12h） | 纠缠协议、密度矩阵、信道；oracle、Fourier/phase estimation、搜索等算法机制 | 解释表示与优化，比较 RL 基础更新，理解量子算法与噪声的作用 |
| M03 | CS285：DQN、PG、actor-critic、PPO/SAC；探索、model-based/offline 概览 | Watrous QEC：syndrome、可纠正性、stabilizer、decoder/logical error；硬件约束与编译模块 B | 分析 RL 稳定性，解释纠错与编译流程；比较一个现成算法或编译设置 |
| M04 | MARL：games、Dec-POMDP、非平稳性、CTDE、信用分配、MAPPO/QMIX | AI for Quantum 模块 C（8h）；主项目选题、论文与最小基线（12h） | 比较单/多智能体建模，确定研究问题、强基线、指标与预算 |
| M05 | IR 模块 A（10h）；PML 推荐主干、内容/序列概览（16h）；系统与评估模块 E（6h） | QUBO/Ising、约束与 penalty、经典求解比较（模块 D，8h）；主项目迭代（12h） | 解释检索推荐流程与评价偏差；验证小规模约束编码 |
| M06 | HF Agents：一个框架、工具、RAG、规划/记忆、失败恢复与评价（24h）；CS285 后训练：SFT、偏好/奖励、RL、reward hacking（8h） | 变分工作流、QAOA/annealing 概览（模块 D，8h）；主项目分析与总结（12h） | 评价 Agent 的正确性与成本，完成项目报告及半年知识回顾 |

每月前沿与复盘 8h 用于关联研究问题、检查理解与更新知识库。

## 每周节奏

| 学习块 | 时间 | 内容 |
| :--- | ---: | :--- |
| 主线阅读 | 3h | 核心章节与知识关系 |
| 主线实践 | 3h | 课程例子、代码阅读或对照实验 |
| 主线复习 | 2h | 先修补缺、概念解释与自检 |
| 量子 / 应用阅读 | 3h | 量子课程、专题材料或项目论文 |
| 量子 / 应用实践 | 2h | 数值例子、建模与主项目 |
| 前沿与复盘 | 2h | 研究关联 1h，周回顾 1h |
| **合计** | **15h** | 可分为每周 5 次、每次 3h |

## 总预算与机动周

**24 个学习周 × 15h = 360h；2 个机动周 × 15h = 30h；总计约 390h。** 六个月按约 26 周估算，实际日期在开始时填写。两个机动周可分别安排在 M03 后和 M06 末，用于补缺、重跑实验和综合回顾。

按章节与知识点选读。ML/RL 基础、态与测量、信道/QEC、评价与经典基线达到可解释和可验证的程度；算法复杂度证明、进阶信息论、model-based/offline RL、CNN/RNN、序列推荐与 annealing 先建立概览，再按项目需要深入。

## 主项目

M01–M03 通过课程例子积累基础；M04 确定一个问题，M04–M06 每月安排 12h 推进，共 36h。候选方向包括学习辅助量子电路搜索/编译和量子优化与约束推荐重排。

项目交付包括：问题定义、可复现的最小基线、至少一次受控比较、结果与限制。复用成熟实现，将时间集中在建模、评价和结果分析。

## 课程导览

每门课从知识地图开始：核心知识 → 模块关系 → 先修知识 → 重点与选读 → 材料版本 → 学习目标。

数学随主题补充，覆盖线性代数、概率、梯度与优化。学习主题包括 ML/DL、RL/MARL、量子信息、QEC/编译、AI for Quantum、IR/RecSys、Agent、后训练和量子优化。后训练关注 SFT、偏好与奖励、策略优化和 reward hacking；研究评价关注数据划分、泛化、强基线及端到端成本。

## 专题阅读入口

| 专题 | 时间 | 入口与重点 |
| :--- | :--- | :--- |
| A · IR | M05 · 10h | [IIR](https://nlp.stanford.edu/IR-book/)第 1–2、6、8、11 章与 15.4；[Retrieve & Re-Rank](https://sbert.net/examples/sentence_transformer/applications/retrieve_rerank/README.html)：BM25、dense retrieval、排序与 Recall/NDCG |
| B · 量子系统与编译 | M03 · 与 QEC 共 20h | Watrous QEC 约 14h；[Qiskit 编译](https://quantum.cloud.ibm.com/docs/en/guides/transpile)约 6h：硬件约束、layout、routing、translation、scheduling |
| C · AI for Quantum | M04 · 8h | [综述](https://arxiv.org/abs/2601.18953)：QAS、控制、校准、解码与编译；按项目选择原始论文深入 |
| D · 量子优化 | M05、M06 各 8h | [QUBO/Ising 建模](https://docs.dwavequantum.com/en/latest/concepts/models.html)、[变分工作流](https://quantum.cloud.ibm.com/learning/en/courses/variational-algorithm-design)、[QAOA](https://arxiv.org/abs/1411.4028)；约束、penalty、annealing 与经典求解比较 |
| E · 推荐系统与评价 | M05 · 6h | [Google 推荐课程](https://developers.google.com/machine-learning/recommendation)：候选生成、two-tower、打分与重排；结合 PML 理解负采样、冷启动、曝光偏差与在线/离线差异 |

专题时间已计入各月预算。资料入口沿用 2026-09-15 的核查记录，开始对应主题时核对材料与工具版本。

## 第一个月详细计划

**本月主题：先建立知识地图，再理解模型与量子系统的基本语言。**

| 项目 | 安排 |
| :--- | :--- |
| 当前状态 | 未开始 |
| 开始日期 | 待实际开始时填写；W1–W4 为相对周 |
| 总预算 | 4 周 × 15h = 60h |
| AI 主线 | D2L：损失、泛化、正则化、分类、MLP 与反传入门 |
| 量子主线 | Watrous：单/多系统、测量、电路与密度矩阵入门 |
| 本月终点 | 能解释模型训练、量子状态、测量与基本电路 |

### 01 · 开课前，先知道课程包含什么

#### D2L 的全局地图

数据与数学工具 → 回归/分类 → MLP/反传 → CNN/RNN → Attention/Transformer → 优化与计算 → 应用。

**本月重点：**模型输入输出、训练/验证/测试、loss 与 metric、泛化、正则化、softmax/cross-entropy、distribution shift。本月进入 MLP 与反传机制；优化、归一化与 Transformer 在 M02 学习。

先修只检查三件事：能读张量形状，理解概率与期望的基本含义，能阅读简单 Python。缺口用 D2L 第 2 章补，计入当周时间。回归部分通过现成例子理解模型流程。

#### Watrous Basics 的全局地图

单系统（态、操作、测量）→ 多系统（张量积、联合测量）→ 电路（门、控制与顺序）→ 纠缠协议（teleportation、superdense coding、CHSH）。

**本月必学：**前三段的核心概念。纠缠重点建立 Bell 态直觉；W4 进入密度矩阵的纯态/混合态表示；纠缠协议与信道在 M02 学习。

General Formulation 的知识地图：密度矩阵 → 量子信道 → 一般测量 → 状态距离。本月从密度矩阵开始，建立后续学习噪声与信道的表示工具。

先修：复数模平方、内积、矩阵作用、张量积的记法。只补当前例子需要的部分。

> 先梳理两门课的核心模块、先修关系与本月重点。

### 02 · 本月固定材料

核查：2026-09-15。D2L 采用官网 1.0.3 文字/代码；Watrous 用当前 IBM 课程文字与其配套视频，统一讲义为 2025 公开版本。视频录制年份不等同于页面更新年份。

| 编号 | 材料 | 本月用途 |
| :--- | :--- | :--- |
| A0 | [D2L 全书目录](https://d2l.ai/) | 第一次课程导览；之后按章节学 |
| A1 | [3.6 Generalization](https://d2l.ai/chapter_linear-regression/generalization.html) | 数据划分、模型复杂度与泛化 |
| A2 | [3.7 Weight Decay](https://d2l.ai/chapter_linear-regression/weight-decay.html) | 正则化的作用与训练/验证表现 |
| A3 | [4.1 Softmax Regression](https://d2l.ai/chapter_linear-classification/softmax-regression.html) | logits、概率输出、cross-entropy |
| A4 | [4.5 Concise Implementation](https://d2l.ai/chapter_linear-classification/softmax-regression-concise.html) | 读现有分类训练流程；需要时查 4.2/4.3 的依赖 |
| A5 | [第 4 章目录](https://d2l.ai/chapter_linear-classification/index.html)中的 4.6/4.7 | 分类泛化与环境/分布变化 |
| A6 | [D2L 全书目录](https://d2l.ai/)中的第 5 章 | MLP、计算图、反向传播与数值稳定性相关节 |
| Q0 | [Basics 总览](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information) | 明确知识地图和先修 |
| Q1 | [Single systems 导览](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/single-systems/introduction) | 通过官方入口看文字、配套视频或 slides，选择一种主媒介 |
| Q2 | [Multiple systems 导览](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/multiple-systems/introduction)及[量子部分](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/multiple-systems/quantum-information) | 张量积、联合状态与测量 |
| Q3 | [Quantum circuits](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/quantum-circuits/circuits) | 操作顺序、控制门、qubit 排序 |
| Q4 | [Watrous 统一讲义](https://arxiv.org/abs/2507.11536) | 与 IBM 课程对应的讲义；W4 选 General Formulation 的密度矩阵入门部分 |

视频和文字选择一种作为主要学习媒介，另一种用于补充解释。D2L 代码阅读围绕数据 → 预测 → 损失 → 更新展开，工具类按需查阅。

### 03 · 每周固定节奏

| 学习块 | 时长 | 内容 |
| :--- | ---: | :--- |
| A | 3h | AI 主阅读 |
| B | 3h | AI 例子、代码阅读与验证 |
| C | 2h | AI 复习与先修补缺 |
| D | 3h | 量子主阅读与概念解释 |
| E | 2h | 量子例子与数值验证 |
| F | 2h | 研究关联 1h + 周复盘 1h |
| **合计** | **15h** | 按个人时间分配到日历 |

阅读、实践和补缺均计入这些学习块。每周可安排五次 3h 学习；A–F 可跨次分配。研究关联围绕“本周概念能解释哪类量子学习问题”展开。

### 04 · W1：课程地图、模型流程与单系统

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 3h | D2L 导览 30min；A1 数据划分、损失与泛化 2.5h | 说明训练/验证/测试的职责与 loss/metric 区别 |
| B · 3h | 浏览第 3 章现成模型；跟踪输入、预测、损失、自动微分、更新与评价 | 画出训练流程，说明参数在何处更新 |
| C · 2h | 检查一个既有实验的数据泄漏风险；按需补张量形状、概率与期望 | 指出数据划分、预处理与模型选择的先后关系 |
| D · 3h | Q0 导览 30min；Q1 状态、操作、测量 2.5h | 区分振幅、概率、unitary 与 measurement |
| E · 2h | 计算归一化与简单单 qubit 操作；用课程数值例子检查测量概率 | 解释操作前后和测量后的状态 |
| F · 2h | 关联泛化与量子实验评价；整理疑问，回顾学习进展 | 记录待补概念与对应来源 |

**自检：**训练 loss 下降为何可能伴随测试表现变差？振幅如何变成测量概率？unitary 与测量对状态的影响有什么区别？

### 05 · W2：分类、正则化与复合系统

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 3h | A2 weight decay 1.5h；A3 softmax/cross-entropy 1.5h | 解释正则化、logits、概率输出与分类损失 |
| B · 3h | 阅读或运行 A4 分类例子；比较 accuracy/loss，观察正则化效果 | 跟踪一个 batch，区分观察与解释 |
| C · 2h | 总结欠拟合/过拟合；补 softmax、cross-entropy 与数据准备中的疑问 | 结合训练和验证结果判断拟合情况 |
| D · 3h | Q2 张量积、基底顺序、产品态、纠缠态与联合测量 | 解释两 qubit 状态的四个振幅和索引 |
| E · 2h | 比较产品态与 Bell 态的联合测量分布 | 区分单系统与联合系统的统计信息 |
| F · 2h | 关联分类评价与联合测量；自检并记录下周先修缺口 | 准备进入 MLP 与量子电路 |

**自检：**更强正则化一定更好吗？loss 与 accuracy 为什么可能不同步？相关性与纠缠有什么关系？

### 06 · W3：MLP、反传与量子电路

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 3h | A6：MLP、非线性激活、计算图与反向传播机制 | 解释层、参数、激活和梯度的作用 |
| B · 3h | 跟踪一个现成 MLP 的 forward、loss、backward、update；观察张量形状与梯度 | 说明梯度累积、清零与参数更新的位置 |
| C · 2h | 复习链式法则的计算图直觉、梯度消失/爆炸与数值稳定性 | 将训练异常对应到可检查的环节 |
| D · 3h | Q3：门、控制门、操作顺序、测量与 qubit 排序 | 逐步解释一个两 qubit 电路 |
| E · 2h | 用现有例子制备 Bell 态，比较理论概率与有限 shots 频率 | 解释电路与测量分布的对应关系 |
| F · 2h | 关联神经网络训练与参数化量子电路；选择 W4 的验证问题 | 写出问题、条件与观察指标 |

**自检：**非线性激活的作用是什么？自动微分计算的梯度用于哪里？矩阵乘法顺序与电路顺序如何对应？

### 07 · W4：训练验证、密度矩阵与月末回顾

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 3h | A5 分类泛化与分布变化 1.5h；复习 A6 训练机制 1.5h | 解释数据变化、模型容量和优化问题的区别 |
| B · 3h | 固定划分与预算，改变正则化强度或模型容量中的一个因素；保存设置与观察 | 完成一次受控比较，说明限制；阅读分析标注来源 |
| C · 2h | AI 月末自检，整理数据→模型→损失→更新→评价的知识关系 | 独立解释完整训练流程与一个失败原因 |
| D · 3h | 先做 General Formulation 知识导览；用 Q4 学纯态密度矩阵、混合态及测量概率 | 解释状态向量与密度矩阵的关系 |
| E · 2h | 比较纯态叠加与经典混合的简单矩阵例子；核对 trace 与测量概率 | 知道同一基底下概率相同的状态仍可能不同 |
| F · 2h | 综合回顾、回顾学习进展、确定 M02 的先修补缺点 | 按月末标准记录掌握情况 |

**自检：**测试分布变化为什么影响结论？纯态与混合态如何表示？只知道一个测量基底下的概率能否确定状态？

### 08 · 月末通过标准

对下列能力标记“能解释 / 需要例子帮助 / 仍不清楚”，并链接自己的记录。

| 能力 | 本月结束时的目标 |
| :--- | :--- |
| ML 任务与评估 | 解释数据划分、loss/metric、泛化与正则化，识别泄漏和分布变化风险 |
| MLP 与训练 | 说明层、激活、计算图、反传与参数更新，能跟踪现成训练代码 |
| 量子基本语言 | 说明振幅/概率、unitary/measurement、多系统与张量积 |
| 电路与纠缠 | 读懂两 qubit 电路，解释 Bell 态、基底顺序与测量分布 |
| 密度矩阵入门 | 读懂纯态与混合态表示，连接状态与测量概率 |
| 实验分析 | 保存一次小验证或有来源的阅读分析，区分观察、解释与待验证部分 |

M02 的 DL 学习以损失、反传和训练/评价为先修；量子信道以密度矩阵和联合系统为先修。自检中的缺口优先安排进下一周对应的复习块，系统性缺口使用机动周。
