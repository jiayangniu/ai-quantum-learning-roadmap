# 一年学习路线

高层方向已确认 · 版本 1.0 · 更新 2026-09-15

[首页](README.md) · [课程与知识地图](COURSES.md) · [第一个月](months/01-foundations/README.md)

## 精简原则

保留 **6 套主资源 + 5 个定向补充模块**。六套是持续使用的教材/课程，不是六个短视频；Watrous 是同一讲义体系的四个单元。补充模块只读指定章节/文档，不增加整门课。

减少重复讲授、平台切换、整套作业和多项目负担；保留原计划的核心知识覆盖。覆盖意味着每个核心主题都有学习入口与理解目标，不表示一年内精通所有细节。

## 六套主资源

| 主资源 | 负责的知识 | 安排 |
|---|---|---|
| 1. D2L | ML/DL、泛化、优化、表示、attention/Transformer | M01–M03 |
| 2. Watrous 量子信息讲义 / IBM 配套课程 | 态/测量/纠缠、算法、密度矩阵/信道、QEC | M01–M05，之后查阅 |
| 3. Berkeley CS285 | Deep RL、PPO/SAC、探索、model-based/offline、LLM RL 概览 | M04–M06；M11 定向回看 |
| 4. MARL Book | RL 基础复习；games、CTDE、credit assignment、deep MARL | M04 用第 2 章；M07–M08 学 MARL |
| 5. Personalized Machine Learning | 推荐、协同过滤、隐因子、内容与序列 | M09–M10 |
| 6. Hugging Face Agents Course | tools、planning、Agentic RAG、evaluation | M11 |

课程链接、开场知识地图及具体选学内容见 [课程指南](COURSES.md)。版本依据见 [版本与来源](MATERIAL_VERSIONS.md)。

## 哪些整门课不再跟？

- Silver 不再从头到尾学；RL 先用 MARL Book 第 2 章。如果 MC/TD 仍不清楚，只用 Silver 对应讲次替代该主题的复读。
- CS229、Preskill、独立数学教材不进入固定日程；只有解释不清某个问题时才查。
- CS276 不整课跟；IIR 只读索引、评分、评价、概率检索与 learning-to-rank 对应部分。
- CSE258 不另看完整视频；PML 为唯一推荐主教材。
- CS336 不额外跟课；后训练先用已在学的 CS285 LLM RL 内容，偏好优化不清楚才查一个对应片段。
- 不全量学习多个 Agent 框架；只选一个。

## 12 个月

| 月 | 主要学习 | 量子 / 应用线 |
|---|---|---|
| M01 | D2L：损失、数据划分、泛化、基础模型 | Watrous：单/多系统、测量、电路 |
| M02 | D2L：MLP、反传机制、优化与正则化 | Watrous：纠缠、密度矩阵、信道 |
| M03 | D2L：attention/Transformer；补确实缺的数学 | Watrous：量子算法代表工具与机制 |
| M04 | MARL Book 第 2 章 RL 基础 → CS285 RL Basics；确认 DP/MC/TD | Watrous：QEC 基础 |
| M05 | CS285：PG、actor-critic、value-based 方法 | QEC stabilizer；编译/硬件约束短模块 |
| M06 | CS285：PPO/SAC、探索；model-based/offline 概览 | AI for Quantum 任务地图与项目选题 |
| M07 | MARL Book：games、局部观测、CTDE、信用分配 | 一篇与主项目直接相关的论文 |
| M08 | MARL Book：MAPPO/QMIX、实践与消融 | 量子主项目最小基线比较 |
| M09 | IIR 指定章节＋dense retrieval 短教程；进入 PML | 继续量子主项目，避免新开项目 |
| M10 | PML：推荐主干、内容/序列概览、评价 | QUBO/Ising 建模短模块 |
| M11 | HF Agents：一个框架、RAG、验证/评估；CS285 后训练回看 | QAOA/变分工作流短模块 |
| M12 | 主项目收尾、知识综合、年度回顾 | AI for Quantum 或量子优化交叉择一深入 |

## 时间与产出

每周约 9h：主线 5h，量子/应用 3h，前沿与回顾 1h。实践和补充阅读计入前两项，不额外加量。48 学习周＋4 机动周；缺口先占机动时间，必要时顺延。

全年只要求 **一个持续演进的主项目**；其他实践为课程内的小例子。第一年可以选量子电路搜索/编译，或者约束推荐重排。没有必要同时交付四个完整项目。

## 每门课的开场保持不变

先说明：包含哪些知识 → 模块间关系 → 你的先修缺口 → 重点/选读 → 教材/视频版本 → 学完能回答的问题。量子从第一月开始；不恢复独立数学月、回归梯度手推或笔记数量打卡。

## 知识覆盖与深度

[课程指南](COURSES.md) 中的覆盖表逐项保留数学、ML、DL、RL、MARL、量子基础、QEC/编译、AI for Quantum、IR/RecSys、Agent 与量子优化。

主线方法需要能解释和评价；其他分支至少建立概念与证据意识。高级证明、大规模硬件、训练大模型和每种算法的完整复现均非首年默认要求。本仓库以这一精简方案为准；后续月份在接近开始时细化，避免维护尚未验证的逐日安排。
