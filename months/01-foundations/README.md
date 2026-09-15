# M01 · ML 与量子基础

**本月主题：先建立知识地图，再理解模型与量子系统的基本语言。**

[首页](../../README.md) · [年度路线](../../ROADMAP.md) · [进度面板](../../PROGRESS.md)

| 项目 | 安排 |
| :--- | :--- |
| 当前状态 | 未开始 |
| 开始日期 | 待实际开始时填写；W1–W4 为相对周 |
| 总预算 | 4 周 × 9h = 36h |
| AI 主线 | D2L：损失、泛化、正则化、分类与评估 |
| 量子主线 | Watrous Basics：单系统、多系统、测量与电路 |
| 本月终点 | 能解释基本机制和结果；不要求完成两本教材 |

## 01 · 开课前，先知道课程包含什么

### D2L 的全局地图

数据与数学工具 → 回归/分类 → MLP/反传 → CNN/RNN → Attention/Transformer → 优化与计算 → 应用。

**本月只取：**模型输入输出、训练/验证/测试、loss 与 metric、泛化、正则化、softmax/cross-entropy、distribution shift。MLP 与完整反传放 M02，Transformer 放 M03。

先修只检查三件事：能读张量形状，理解概率与期望的基本含义，能阅读简单 Python。缺口用 D2L 第 2 章补，计入当周时间。熟悉回归者直接浏览例子，不做梯度手推。

### Watrous Basics 的全局地图

单系统（态、操作、测量）→ 多系统（张量积、联合测量）→ 电路（门、控制与顺序）→ 纠缠协议（teleportation、superdense coding、CHSH）。

**本月必学：**前三段的核心概念。纠缠先到 Bell 态直觉；完整协议自然延续到 M02，不挤占基本理解。密度矩阵/信道是下一阶段，不提前塞进本月。

先修：复数模平方、内积、矩阵作用、张量积的记法。只补当前例子需要的部分。

> 第一项学习活动是说明两门课分别包含什么、为什么这样安排；不是立即开始看视频。使用 [课程导览模板](../../templates/course-orientation.md)。

## 02 · 本月固定材料

核查：2026-09-15。D2L 采用官网 1.0.3 文字/代码；Watrous 用当前 IBM 课程文字与其配套视频，统一讲义为 2025 公开版本。视频录制年份不等同于页面更新年份。

| 编号 | 材料 | 本月用途 |
| :--- | :--- | :--- |
| A0 | [D2L 全书目录](https://d2l.ai/) | 第一次课程导览；之后按章节学 |
| A1 | [3.6 Generalization](https://d2l.ai/chapter_linear-regression/generalization.html) | 数据划分、模型复杂度与泛化 |
| A2 | [3.7 Weight Decay](https://d2l.ai/chapter_linear-regression/weight-decay.html) | 正则化的作用与训练/验证表现 |
| A3 | [4.1 Softmax Regression](https://d2l.ai/chapter_linear-classification/softmax-regression.html) | logits、概率输出、cross-entropy |
| A4 | [4.5 Concise Implementation](https://d2l.ai/chapter_linear-classification/softmax-regression-concise.html) | 读现有分类训练流程；需要时查 4.2/4.3 的依赖 |
| A5 | [第 4 章目录](https://d2l.ai/chapter_linear-classification/index.html)中的 4.6/4.7 | 分类泛化与环境/分布变化 |
| Q0 | [Basics 总览](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information) | 明确知识地图和先修 |
| Q1 | [Single systems 导览](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/single-systems/introduction) | 通过官方入口看文字、配套视频或 slides，选择一种主媒介 |
| Q2 | [Multiple systems 导览](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/multiple-systems/introduction)及[量子部分](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/multiple-systems/quantum-information) | 张量积、联合状态与测量 |
| Q3 | [Quantum circuits](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/quantum-circuits/circuits) | 操作顺序、控制门、qubit 排序 |
| Q4 | [Watrous 统一讲义](https://arxiv.org/abs/2507.11536) | 网页不便时使用的替代阅读入口，不重复跟读 |

本月不增加新课程。视频和文字选择一个为主，另一个只补没看懂的段落。D2L 的工具类若影响理解，先读数据→预测→损失→更新的流程，不花整周重写教材框架。

## 03 · 每周固定节奏

| 学习块 | 时长 | 内容 |
| :--- | ---: | :--- |
| A | 2h | AI 主阅读 |
| B | 2h | AI 例子/对照/代码阅读 |
| C | 1h | AI 回顾与缺口 |
| D | 1.5h | 量子主阅读/视频 |
| E | 1.5h | 量子例子与问题 |
| F | 1h | 前沿定位 0.5h + 周复盘 0.5h |
| **合计** | **9h** | 自行分配到日历，不要求每天打卡 |

前沿定位可以是“这个基础概念将用于哪类问题”，不要求读一篇新论文。忙碌周优先保留课程理解，缩小例子；积压不靠下周翻倍补。

## 04 · W1：建立地图，理解模型与单系统

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 2h | D2L 导览 30min；A1 读训练/验证/测试和泛化 90min | 能说清三个数据集各自的职责 |
| B · 2h | 从 D2L 第 3 章浏览一个现成模型流程；指出输入、预测、损失、更新和评价 | 能指出优化目标与最终指标的区别；不用手推梯度 |
| C · 1h | 对照自己过去的一个实验，检查是否反复利用测试集或先全量预处理再划分 | 写出一个具体风险或一个正确设计 |
| D · 1.5h | Q0 导览 30min；Q1 的状态/测量 60min | 知道向量中的振幅与测量概率不同 |
| E · 1.5h | 继续 Q1：归一化、unitary、简单单 qubit 操作；必要时补复数模平方 | 能解释操作前后与测量后的状态各是什么 |
| F · 1h | 定位泛化与测量在量子学习中的作用；记录最不清楚的问题 | 下一周有明确补缺点 |

**自检：**为什么训练 loss 下降不等于测试表现提高？振幅能否直接当概率？“知道测量分布”是否等于“知道每次测量结果”？

## 05 · W2：泛化、正则化与复合系统

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 2h | A1 补完需要部分 → A2 的正则化解释 | 能说明正则化改变了什么 |
| B · 2h | 看 A2 示例中的训练/验证趋势；有可用环境则只改变正则化强度，否则先解释现有图表 | 区分观察、假设与尚未验证的解释 |
| C · 1h | 总结 underfit/overfit 的判断；核对数据划分、训练预算等条件 | 不仅凭一条训练曲线下结论 |
| D · 1.5h | Q2：从单系统到多系统；张量积与基底顺序 | 能读懂两 qubit 状态的索引 |
| E · 1.5h | 产品态与纠缠态、联合测量的例子；卡住则先补张量积 | 能解释联合结果与各个系统结果的关系 |
| F · 1h | 回顾泛化与联合系统；只保留重要问题和来源 | 决定 W3 是否需要多系统补课 |

**自检：**更强正则化一定更好吗？两个 qubit 的四个振幅分别表示什么？相关性是否自动意味着纠缠？最后一问可以先标记待深入。

## 06 · W3：分类与量子电路

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 2h | A3：logits → softmax → cross-entropy；熟悉的代数推导可略读 | 能说明输出、损失与预测标签之间的关系 |
| B · 2h | A4：阅读或运行现成分类示例；按需查数据准备与类定义 | 能跟踪一个 batch 的完整路径 |
| C · 1h | 比较 accuracy 与 loss；思考类别不平衡、过度自信等情况 | 能给出二者不一致的例子 |
| D · 1.5h | Q3：线、门、测量、操作顺序与控制门 | 能逐步口述一个小电路 |
| E · 1.5h | Bell 态制备例子；关注 Qiskit 的 bit/qubit 排序约定 | 不把显示顺序误解成物理差异 |
| F · 1h | 连接分类评估与量子实验观察；记录下周想检验的一个问题 | 保持一项小验证，不开新项目 |

**自检：**为什么输出概率与准确率不是同一件事？电路的左右顺序与矩阵乘法顺序如何对应？量子寄存器显示顺序为何重要？

## 07 · W4：整合、一个小验证与月末回顾

| 块 | 具体安排 | 完成标志 |
| :--- | :--- | :--- |
| A · 2h | A5 中 4.6/4.7：分类泛化与分布变化 | 能解释部署数据变化为何使评估失效 |
| B · 2h | 选择一个小验证：固定划分后改正则化，或分析同一模型的 loss/accuracy；不同时改多个因素 | 保存设置、观察、限制；未运行就明确写“阅读分析” |
| C · 1h | AI 月末回顾：画自己的流程图，回看最初的疑问 | 能从任务讲到评价而不依赖逐行读代码 |
| D · 1.5h | 完成 Q1–Q3 缺口，复习产品态/纠缠/测量 | 能解释一个两 qubit 电路及其结果分布 |
| E · 1.5h | 用现有 notebook 或简单数值例子核对 Bell 态；若基础未稳则用课程例子解释 | 区分理论概率与有限 shots 的频率；噪声留待后续 |
| F · 1h | 月末检查、更新进度、给 M02 留出最弱先修点 | 决定继续或补一周，不自动标记完成 |

**本月不强求：**完整量子通信协议、CHSH 证明、MLP/Transformer、完整 QEC、独立研究论文复现。

## 08 · 月末通过标准

不按笔记数量评分。请对下列问题标为“能解释 / 需要例子帮助 / 仍不清楚”，并链接自己的记录。

| 能力 | 本月结束时的目标 |
| :--- | :--- |
| ML 任务与评估 | 说明数据划分、loss/metric、泛化与正则化；识别一个泄漏或分布变化风险 |
| 模型流程 | 看懂现成训练例子的关键环节，不需要从零写出框架 |
| 量子基本语言 | 说明振幅/概率、unitary/measurement、多系统与张量积 |
| 电路理解 | 读懂一个两 qubit 电路，解释基底/显示顺序和测量分布 |
| 证据意识 | 区分亲自运行、教材结果和自己的推测 |

若 ML 或单/多系统基础仍不清楚，用机动周补对应主题。进入 M02 的 General Formulation 前应理解基本测量与联合系统；进入 MLP 前应理解损失与训练/评价的区别。

## 09 · 最简记录方式

- 日常问题和概念放 [notes](../../notes/README.md)，按主题保存，月份文档只链接它们。
- 真正运行过的验证放 [experiments](../../experiments/README.md)；没有运行就不填结果。
- 每周只更新一次 [PROGRESS](../../PROGRESS.md)，日期按实际填写。
- 本月开始前无需购买课程、申请硬件、训练大模型或安装所有后续工具。
