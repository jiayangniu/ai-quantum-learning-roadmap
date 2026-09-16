# AI × Quantum · 半年学习索引

**6 个月 · 每周 15 小时 · 24 个学习周 + 2 个机动周 · 约 390 小时**

[半年索引](#半年索引) · [课程目录](#课程目录) · [首月周索引](#首月周索引)

## 半年索引

| 月份 | 知识点 | 教材 / 课程 |
| :--- | :--- | :--- |
| M01 | ML 基础、MLP、反传；量子态、测量、电路、密度矩阵入门 | D2L 第 3–5 章；Watrous Basics、General Formulation |
| M02 | 优化、归一化、CNN/RNN、Attention/Transformer；MDP、DP/MC/TD；信道、纠缠协议、量子算法 | D2L 第 5–12 章相关节；MARL 第 2 章、CS285 RL Basics；Watrous General Formulation、Basics、Algorithms |
| M03 | DQN、PG、Actor-Critic、PPO/SAC、探索、Model-based/Offline RL；QEC、硬件约束、编译 | CS285；Watrous QEC；Qiskit Transpilation |
| M04 | Games、Dec-POMDP、CTDE、信用分配、MAPPO/QMIX；QAS、控制、校准、解码、编译 | MARL 第 3–6、9–11 章；AI for Quantum 综述 |
| M05 | IR、协同过滤、隐因子、内容/序列推荐、系统评价；QUBO/Ising、约束与经典基线 | IIR、Retrieve & Re-Rank；PML 第 4–7 章；Google 推荐课程；D-Wave Models |
| M06 | Tools、RAG、Planning、Memory、Evaluation；SFT、偏好/奖励、RL；变分算法、QAOA、Annealing | HF Agents Unit 1–3、Evaluation；CS285 LLM RL；IBM 变分算法、QAOA、D-Wave Models |

主项目：M04–M06，每月 12h，计入每周预算；方向为量子电路搜索/编译或约束推荐重排。

## 课程目录

| 教材 / 课程 | 知识地图与章节 |
| :--- | :--- |
| [D2L · 1.0.3](https://d2l.ai/) | 数据与数学（第 2 章）→ 回归/分类、泛化（第 3–4 章）→ MLP/反传（第 5 章）→ CNN/RNN、归一化（第 7–10 章选读）→ Attention/Transformer（第 11 章）→ 优化（第 12 章） |
| [Watrous · 2025 讲义](https://arxiv.org/abs/2507.11536) / [IBM 课程](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information) | Basics：单/多系统、测量、电路、纠缠协议 → General Formulation：密度矩阵、信道、一般测量、状态距离 → Algorithms：Oracle、Fourier/Phase Estimation、搜索 → QEC：编码、错误离散化、可纠正性、Syndrome/Stabilizer |
| [CS285 · 2026 课件](https://rail.eecs.berkeley.edu/deeprlcourse/) | RL Basics → PG/Actor-Critic → Q-learning → PPO/SAC → 探索、Model-based/Offline RL → LLM RL；2023 录像对应基础主题 |
| [MARL Book · 2024](https://www.marl-book.com/) | RL 基础（第 2 章）→ Games、多智能体挑战与基础算法（第 3–6 章）→ Deep MARL（第 9–10 章）→ 环境（第 11 章） |
| [Personalized Machine Learning · 2022](https://cseweb.ucsd.edu/~jmcauley/pml/) | 协同过滤、隐因子（第 4–5 章）→ 内容、结构、时间与序列（第 6–7 章选读） |
| [HF Agents](https://huggingface.co/learn/agents-course/en/unit0/introduction) | 基础（Unit 1）→ 一个框架（Unit 2）→ Agentic RAG（Unit 3）→ Evaluation Bonus |

### 专题入口

| 知识点 | 教材位置 |
| :--- | :--- |
| 索引、BM25、检索评价、Learning to Rank | [IIR](https://nlp.stanford.edu/IR-book/)第 1–2、6、8、11 章及 §15.4 |
| Dense Retrieval、Re-ranking | [Retrieve & Re-Rank](https://sbert.net/examples/sentence_transformer/applications/retrieve_rerank/README.html) |
| 候选生成、Two-tower、打分、重排 | [Google Recommendation Systems](https://developers.google.com/machine-learning/recommendation) |
| 负采样、冷启动、曝光偏差、在线/离线评价 | PML 第 4–7 章；IIR 第 8 章；Google Recommendation Systems |
| Layout、Routing、Translation、Scheduling | [Qiskit Transpilation](https://quantum.cloud.ibm.com/docs/en/guides/transpile) |
| QAS、控制、校准、解码、编译 | [RL for Quantum Technology · 2026 综述](https://arxiv.org/abs/2601.18953) |
| QUBO、Ising、Penalty、Annealing | [D-Wave Models](https://docs.dwavequantum.com/en/latest/concepts/models.html) |
| Cost、Ansatz、Measurement、Optimizer | [IBM Variational Algorithm Design](https://quantum.cloud.ibm.com/learning/en/courses/variational-algorithm-design) |
| QAOA | [原始论文](https://arxiv.org/abs/1411.4028) |
| SFT、偏好优化、奖励、RL、Reward Hacking | CS285 LLM RL；[CS336 · 2026 后训练](https://cs336.stanford.edu/)对应讲次 |

## 首月周索引

### W1 · ML 与单量子系统

| 知识点 | 教材位置 |
| :--- | :--- |
| 课程知识地图 | [D2L 目录](https://d2l.ai/)；[Watrous Basics 目录](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information) |
| 数据划分、损失、泛化 | [D2L §3.6 Generalization](https://d2l.ai/chapter_linear-regression/generalization.html) |
| 模型与训练流程 | D2L 第 3 章：Linear Neural Networks for Regression |
| 张量形状、概率、自动微分 | D2L 第 2 章：Preliminaries |
| 量子态、振幅、概率、Unitary、测量 | [Watrous Basics · Single Systems](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/single-systems/introduction) |

### W2 · 分类与复合量子系统

| 知识点 | 教材位置 |
| :--- | :--- |
| 正则化、Weight Decay | [D2L §3.7 Weight Decay](https://d2l.ai/chapter_linear-regression/weight-decay.html) |
| Logits、Softmax、Cross-entropy | [D2L §4.1 Softmax Regression](https://d2l.ai/chapter_linear-classification/softmax-regression.html) |
| 分类训练、Loss 与 Accuracy | [D2L §4.5 Concise Implementation](https://d2l.ai/chapter_linear-classification/softmax-regression-concise.html) |
| 张量积、产品态、纠缠态、联合测量 | [Watrous Basics · Multiple Systems](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/multiple-systems/quantum-information) |

### W3 · MLP 与量子电路

| 知识点 | 教材位置 |
| :--- | :--- |
| MLP、非线性激活 | [D2L §5.1–5.2 · Multilayer Perceptrons](https://d2l.ai/chapter_multilayer-perceptrons/index.html) |
| 计算图、反向传播、梯度累积与更新 | [D2L §5.3 · Forward/Backward Propagation](https://d2l.ai/chapter_multilayer-perceptrons/index.html)；§2.5 Automatic Differentiation |
| 梯度消失/爆炸、数值稳定性 | [D2L §5.4 · Numerical Stability and Initialization](https://d2l.ai/chapter_multilayer-perceptrons/index.html) |
| 量子门、控制门、操作顺序、Qubit 排序、Bell 态电路 | [Watrous Basics · Quantum Circuits](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/quantum-circuits/circuits) |

### W4 · 分布变化与密度矩阵

| 知识点 | 教材位置 |
| :--- | :--- |
| 分类泛化、分布变化 | [D2L 第 4 章](https://d2l.ai/chapter_linear-classification/index.html) §4.6 Generalization in Classification、§4.7 Environment and Distribution Shift |
| 模型容量、正则化与训练机制 | D2L §3.6–3.7、第 5 章 |
| General Formulation 知识地图 | [Watrous 讲义](https://arxiv.org/abs/2507.11536)：General Formulation of Quantum Information |
| 纯态密度矩阵、混合态、Trace、测量概率 | Watrous General Formulation：Density Matrices |
