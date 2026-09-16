# 六套主资源与知识覆盖

本指南列出各课程的知识地图、学习范围、先修与目标。材料核查日期：2026-09-15。

## 1. D2L：AI 基础主教材

**先看知识地图：**数据/概率/自动微分 → 回归与分类 → 泛化/正则化 → MLP/反传 → 优化 → CNN/RNN/attention/Transformer → 应用与计算性能。

[官方教材](https://d2l.ai/)，当前页面标记 1.0.3。M01–M02 主读第 3–5、11、12 章相关部分；第 2 章按需回查，CNN/RNN 以机制概览为主。

先修：基本 Python 和矩阵记法；不足时在同一本书内补。回归部分重点阅读模型与训练流程。目标：看懂训练与表示机制，解释泛化、优化和评估问题。

## 2. Watrous：统一量子主教材

**先看四个单元的知识地图：**

- Basics：状态/操作/测量 → 多系统/张量积 → 电路 → 纠缠与通信协议。
- General Formulation：密度矩阵 → quantum channels → general measurements → 状态距离/相似性。
- Algorithms：oracle/query → 代表性量子算法工具 → Fourier/phase estimation、搜索与分解。
- QEC：编码/错误 → 错误离散化与可纠正性 → syndrome/stabilizer。

[2025 统一讲义](https://arxiv.org/abs/2507.11536) 为主，[IBM 系列入口](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information) 提供文字与配套视频。每个单元以知识导览开始，明确概念之间的关系。

M01–M03 学以上核心，算法复杂度证明与进阶信息论后置。先修：复数、内积、概率；遇到再补。噪声与 QEC 是量子主线的核心主题。

## 3. CS285：RL 方法主课程

**先看知识地图：**imitation/RL basics → policy gradient/actor-critic → Q-learning → advanced PG → inference/LLM RL → model-based/offline RL → exploration/multi-task。

[2026 官网](https://rail.eecs.berkeley.edu/deeprlcourse/)为主课件；2023 录播用于同主题基础概念的补充。M02 用 12h 建立 RL 基础（含 MARL Book 第 2 章），M03 学核心算法；model-based/offline 先读概览。M06 回看第 14 讲 LLM RL，连接 SFT、奖励、策略优化与 Agent 训练。偏好优化需更具体材料时才查 [CS336 2026 后训练](https://cs336.stanford.edu/)的对应部分。

**基础准备：**用 MARL Book 第 2 章学习 MDP/value/control，并检查 DP、MC、TD、on/off-policy 与探索的理解。需要补充解释时，阅读 [Silver](https://davidstarsilver.wordpress.com/teaching/)第 2–5 讲中的对应内容。

先修：概率、神经网络训练。目标：解释 PPO/SAC 等设计与训练稳定性，能判断预算、奖励与评估是否合理。

## 4. MARL Book：多智能体主教材

**先看知识地图：**RL 复习 → games/solution concepts → 多智能体学习挑战 → 基础算法 → DL/RL 复习 → deep MARL → 实践与环境。

[作者官网](https://www.marl-book.com/)提供 2024 教材的修订 PDF、slides、视频与练习。M02 学第 2 章；M04 选第 3–6、9–10 章，第 11 章只选一个环境。第 7–8 章用于查阅 DL/RL 基础。

先修：单智能体 RL。重点：Markov games、Dec-POMDP、CTDE、非平稳性、credit assignment、MAPPO/QMIX、执行信息限制。目标：判断多 agent 方法的适用条件与代价。

## 5. Personalized Machine Learning：推荐主教材

**先看知识地图：**预测任务复习 → 协同/隐因子推荐 → 内容与结构 → 时间与序列 → 文本等数据表示。

[作者公开教材](https://cseweb.ucsd.edu/~jmcauley/pml/)为推荐主教材；[CSE258 2025](https://cseweb.ucsd.edu/classes/fa25/cse258-a/)只用于查章节映射。M05 主读第 4–5 章，第 6–7 章保留关键概念；第 2–3 章用于查阅 ML 基础。

先修：ML/DL 与评价。重点：collaborative filtering、latent factors、implicit feedback、内容/序列、冷启动。负采样、数据划分、曝光偏差与在线/离线差异是贯穿阅读的检查项，缺解释时只补对应主题。

## 6. Hugging Face Agents：Agent 实践主课程

**先看知识地图：**tools/actions/observations → 框架 → Agentic RAG → 项目 → function calling、observability/evaluation 等 bonus。

[当前官方课程](https://huggingface.co/learn/agents-course/en/unit0/introduction)：Unit 1 → Unit 2 选一个框架 → Unit 3 → evaluation bonus。M06 学习，在一个框架中完成工具调用、检索与评价实践。

先修：Python、LLM 基础、检索。重点：工具、规划、记忆、验证、失败恢复与任务评价。后训练结合 CS285 学习，并区分工具调用、策略学习与多智能体协作。

## 五个专题模块

各模块围绕知识地图选读指定章节，并通过课程例子或主项目连接理论与应用。

| 模块 | 先看知识地图 | 固定入口与范围 |
|---|---|---|
| A. IR 与现代检索 | 索引 → scoring/BM25 → evaluation → learning to rank → dense retrieval/re-ranking | [IIR](https://nlp.stanford.edu/IR-book/)第 1–2、6、8、11 章相关节及 15.4 learning to rank；第 7 章只补效率。接一个 [Retrieve & Re-Rank](https://sbert.net/examples/sentence_transformer/applications/retrieve_rerank/README.html) 教程 |
| B. 量子系统与编译 | 硬件约束 → layout/routing/translation → scheduling → 噪声与成本 | [Qiskit transpilation](https://quantum.cloud.ibm.com/docs/en/guides/transpile)的管线与一个设置比较示例；QEC 本体已在 Watrous，decoder 数据流不清楚时才看 Stim/PyMatching 小例子 |
| C. AI for Quantum | quantum task → observation/action/reward → baseline → generalization → deployment constraints | [2026 综述](https://arxiv.org/abs/2601.18953)先做地图；[量子反馈](https://arxiv.org/abs/1802.05267)或[QEC 控制](https://www.nature.com/articles/s41586-026-10759-2)按项目深读一篇。QAS/控制/校准/解码/编译先全览，择一深入 |
| D. 量子优化 × IR/RecSys | QUBO/Ising/penalty → cost/ansatz/measurement/optimizer → QAOA/annealing → 经典比较 | [D-Wave Models](https://docs.dwavequantum.com/en/latest/concepts/models.html)读建模；[IBM 变分算法](https://quantum.cloud.ibm.com/learning/en/courses/variational-algorithm-design)只读工作流与关键组件；[QAOA](https://arxiv.org/abs/1411.4028)看机制；小问题通过枚举验证，并与经典求解方法比较 |
| E. 检索推荐的系统与评估 | 候选生成 → two-tower/表示 → scoring/re-ranking → 偏差、成本与线上/离线差异 | [Google 推荐课程](https://developers.google.com/machine-learning/recommendation)只读候选生成、打分、重排，与模块 A 及 PML 关联；指标、负采样、曝光偏差逐项解释，未解释清楚的标成待补 |

## 专题时间安排

| 模块 | 阶段与预算 | 阅读目标 |
| :--- | :--- | :--- |
| A. IR | M05 · 10h | 索引、BM25、排序、评价与 dense retrieval 流程 |
| B. 量子系统与编译 | M03 · 与 QEC 共 20h | QEC 核心约 14h，编译与硬件约束约 6h |
| C. AI for Quantum | M04 · 8h | 任务地图与原始论文导读，项目深读计入项目时间 |
| D. 量子优化 | M05 · 8h；M06 · 8h | 先学编码与经典比较，再学变分工作流、QAOA 与 annealing 概览 |
| E. 系统与评估 | M05 · 6h | 候选生成、打分、重排与评价偏差 |

以上时间已计入 [半年路线](ROADMAP.md)，包含相关例子与复习。每门主课程的实践同样计入所属月份预算。

## 核心知识覆盖检查

下表将核心主题对应到学习材料和理解目标。各主题的进展记录在 [进度面板](PROGRESS.md)，深入范围由主项目确定。

| 核心主题 | 学习材料 | 要达到的理解 |
|---|---|---|
| 数学：线代、概率、梯度、优化 | D2L 第 2/12 章＋Watrous 数学记法 | 能读公式、变量形状和假设 |
| ML：损失、泛化、正则化、评估 | D2L | 能区分模型、数据和评估问题 |
| DL：反传、归一化、优化、attention | D2L，对缺失小节定向回查 | 能解释训练与表示机制 |
| RL：MDP/DP/MC/TD、DQN/PG/AC、PPO/SAC | MARL 第 2 章＋CS285；Silver 对应概念按需 | 理解样本、奖励、偏差方差与稳定性 |
| 现代 RL：offline/model-based、探索 | CS285 对应讲次概览 | 理解适用条件，主项目需要时深入 |
| MARL：Dec-POMDP/CTDE、信用分配、MAPPO/QMIX | MARL Book | 能解释信息约束、协调与复杂度 |
| 量子：态、测量、纠缠、算法、密度矩阵、信道 | Watrous 四单元中的前三个 | 能理解量子任务和噪声假设 |
| QEC/系统/编译：syndrome、decoder、logical error、routing | Watrous QEC＋模块 B | 区分纠错、解码、控制与编译；解释资源约束 |
| AI for Quantum：QAS、控制、校准、解码、编译 | 模块 C＋主项目 | 全览任务区别，选一个问题深入 |
| IR：BM25、dense retrieval、ranking、Recall/NDCG | 模块 A/E | 建立公平检索评价与成本意识 |
| RecSys：MF、two-tower、负采样、序列、冷启动/偏差 | PML＋模块 A/E | 连接建模、数据与系统评价 |
| Agent：tool/RAG/planning/memory/verification/evaluation | HF＋检索模块 | 区分组件作用，评价正确性、失败与成本 |
| Post-training：SFT、偏好/奖励、RL、reward hacking | CS285 LLM RL；必要时 CS336 对应片段 | 理解训练目标、奖励设计与评价的关系 |
| 量子优化：QUBO/Ising、QAOA/annealing、约束重排 | 模块 D＋PML | 通过经典基线验证编码、可行率和端到端成本 |
