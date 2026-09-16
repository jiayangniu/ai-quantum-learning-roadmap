# 一年学习路线

学习周期：12 个月 · 更新 2026-09-16

[首页](README.md) · [课程与知识地图](COURSES.md) · [第一个月](months/01-foundations/README.md)

## 学习目标

通过 **6 套主资源与 5 个专题模块**，建立 AI、量子系统、检索推荐与智能体的知识框架。主线方法以能够解释机制、设计实验和评价结果为目标；交叉领域先建立任务地图，再围绕主项目深入。

## 六套主资源

| 主资源 | 负责的知识 | 安排 |
|---|---|---|
| 1. D2L | ML/DL、泛化、优化、表示、attention/Transformer | M01–M03 |
| 2. Watrous 量子信息讲义 / IBM 配套课程 | 态/测量/纠缠、算法、密度矩阵/信道、QEC | M01–M05，之后查阅 |
| 3. Berkeley CS285 | Deep RL、PPO/SAC、探索、model-based/offline、LLM RL 概览 | M04–M06；M11 定向回看 |
| 4. MARL Book | RL 基础复习；games、CTDE、credit assignment、deep MARL | M04 用第 2 章；M07–M08 学 MARL |
| 5. Personalized Machine Learning | 推荐、协同过滤、隐因子、内容与序列 | M09–M10 |
| 6. Hugging Face Agents Course | tools、planning、Agentic RAG、evaluation | M11 |

课程链接、知识地图及具体选学内容见 [课程指南](COURSES.md)。版本依据见 [版本与来源](MATERIAL_VERSIONS.md)。

## 12 个月

| 月 | 主要学习 | 量子 / 应用线 |
|---|---|---|
| M01 | D2L：损失、数据划分、泛化、基础模型 | Watrous：单/多系统、测量、电路 |
| M02 | D2L：MLP、反传机制、优化与正则化 | Watrous：纠缠、密度矩阵、信道 |
| M03 | D2L：attention/Transformer；相关数学工具 | Watrous：量子算法代表工具与机制 |
| M04 | MARL Book 第 2 章 RL 基础 → CS285 RL Basics；确认 DP/MC/TD | Watrous：QEC 基础 |
| M05 | CS285：PG、actor-critic、value-based 方法 | QEC stabilizer；编译/硬件约束短模块 |
| M06 | CS285：PPO/SAC、探索；model-based/offline 概览 | AI for Quantum 任务地图与项目选题 |
| M07 | MARL Book：games、局部观测、CTDE、信用分配 | 一篇与主项目直接相关的论文 |
| M08 | MARL Book：MAPPO/QMIX、实践与消融 | 量子主项目最小基线比较 |
| M09 | IIR 指定章节＋dense retrieval 短教程；进入 PML | 量子主项目迭代 |
| M10 | PML：推荐主干、内容/序列概览、评价 | QUBO/Ising 建模短模块 |
| M11 | HF Agents：一个框架、RAG、验证/评估；CS285 后训练回看 | QAOA/变分工作流短模块 |
| M12 | 主项目收尾、知识综合、年度回顾 | AI for Quantum 或量子优化交叉择一深入 |

## 时间与产出

每周约 9h：主线 5h，量子/应用 3h，前沿与回顾 1h。实践和补充阅读计入对应学习线。48 学习周＋4 机动周；缺口先占机动时间，必要时顺延。

全年围绕 **一个持续演进的主项目** 积累实践结果，课程例子用于验证具体概念。候选方向包括量子电路搜索/编译和约束推荐重排。

## 课程导览

每门课从知识地图开始：核心知识 → 模块关系 → 先修知识 → 重点与选读 → 材料版本 → 学习目标。使用 [课程导览模板](templates/course-orientation.md) 记录。

## 知识覆盖与深度

[课程指南](COURSES.md) 中的覆盖表对应数学、ML、DL、RL、MARL、量子基础、QEC/编译、AI for Quantum、IR/RecSys、Agent 与量子优化。

主线方法需要能解释和评价；其他分支建立概念框架与证据意识。深入内容由主项目的问题决定。每月根据学习结果细化下一阶段的章节、实践与复习安排。
