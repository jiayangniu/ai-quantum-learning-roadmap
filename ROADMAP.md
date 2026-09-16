# 半年学习路线

学习周期：6 个月 · 每周 15 小时 · 更新 2026-09-16

[首页](README.md) · [课程与知识地图](COURSES.md) · [第一个月](months/01-foundations/README.md)

## 学习目标

通过 **6 套主资源与 5 个专题模块**，建立 AI、量子系统、检索推荐与智能体的知识框架。主线方法以能够解释机制、设计实验和评价结果为目标；交叉领域先建立任务地图，再围绕主项目深入。

## 六套主资源

| 主资源 | 核心知识 | 学习阶段 |
| :--- | :--- | :--- |
| D2L | ML/DL、泛化、反传、优化、表示、attention/Transformer | M01–M02 |
| Watrous / IBM 量子系列 | 态、测量、纠缠、密度矩阵、信道、算法、QEC | M01–M03 |
| Berkeley CS285 | PG/actor-critic、DQN、PPO/SAC、探索、model-based/offline RL | M02 基础准备；M03 核心方法；M06 后训练 |
| MARL Book | MDP、games、Dec-POMDP、CTDE、信用分配、MAPPO/QMIX | M02 第 2 章；M04 多智能体 |
| Personalized Machine Learning | 协同过滤、隐因子、隐式反馈、内容与序列推荐 | M05 |
| Hugging Face Agents | 工具、规划、记忆、Agentic RAG、验证与评价 | M06 |

课程的知识地图、先修和选读章节见 [课程指南](COURSES.md)，材料版次见 [版本档案](MATERIAL_VERSIONS.md)。

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

## 课程导览与知识库

每门课从知识地图开始：核心知识 → 模块关系 → 先修知识 → 重点与选读 → 材料版本 → 学习目标。使用 [课程导览模板](templates/course-orientation.md) 记录。

[课程指南](COURSES.md#核心知识覆盖检查) 将数学、ML、DL、RL、MARL、量子基础、QEC/编译、AI for Quantum、IR/RecSys、Agent 与量子优化对应到材料和理解目标。按主题保存概念与实验，每月根据学习结果细化下一阶段安排。
