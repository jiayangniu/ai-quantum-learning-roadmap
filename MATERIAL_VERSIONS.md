# 教材、课程与视频：版本档案

核查日期：**2026-09-15**。选材原则：经典基础建立长期框架；快速变化的方法、工具和后训练内容采用较新的官方材料。

教材版次、课件年份与录像年份分别记录。视频可用性以表中的核查说明为准。

## 使用范围

主资源为 D2L、Watrous、CS285、MARL Book、PML、HF Agents。专题阅读范围见 [课程指南](COURSES.md)，其余材料作为概念与理论参考。

参考用途：CS229、Preskill、MML 用于理论与数学查阅；Silver 与 Sutton & Barto 用于 RL 基础；CS336 用于后训练；CS276/CSE258 用于章节映射。

## 来源版本档案

| 材料 | 选用版本/类型 | 教材与视频安排 | 为什么选它 / 边界 |
|---|---|---|---|
| [D2L](https://d2l.ai/) | 成熟系统教材；官网当前标记 1.0.3 | 在线教材/代码为主 | 用统一框架串起模型与训练 |
| [CS229 notes](https://cs229.stanford.edu/main_notes.pdf) | PDF 标注 2026-08-23 | 公开讲义为主 | 经典 ML 体系的较新讲义，补泛化、表示学习等理论 |
| [MML](https://mml-book.github.io/) | 2020 出版；作者在线 PDF/勘误入口 | 数学查阅 | 覆盖稳定的数学基础；查阅时记录下载版本 |
| [Watrous 系列统一讲义](https://arxiv.org/abs/2507.11536) | 2025 arXiv 公开讲义；IBM 当前课程页 | Basics / General Formulation / Algorithms / QEC 各自使用官网文字与配套视频入口 | 系统、较新且连贯；视频具体录制年未逐一确认 |
| [Preskill Ph219](https://www.preskill.caltech.edu/ph219/) | 经典讲义，逐章更新 | QEC 第 7 章网页标为 2026-03；第 2–3 章为 2015；2020 录播仅对应第 1–6 章 | 经典理论补充；QEC 采用对应新版讲义 |
| [Silver RL](https://davidstarsilver.wordpress.com/teaching/) | 2015 经典公开课 | 使用作者官网提供的视频与 slides | MDP/TD/PG 的基础结构清楚；PPO/SAC/LLM RL 由后续课程补 |
| [Sutton & Barto](https://mitpress.mit.edu/9780262352703/reinforcement-learning/) | 第二版，2018，经典教材 | 作为定义与理论参考；视频由 Silver 承担 | 用于 RL 定义与理论查阅 |
| [CS285/185](https://rail.eecs.berkeley.edu/deeprlcourse/) | 官网当前为 Spring 2026 | **主用 2026 讲义**；官网列出的 2023 录播只用于重合基础主题的补充 | 新课件覆盖 LLM/offline/model-based RL；录像按主题对应课件 |
| [MARL Book](https://www.marl-book.com/) | 2024 出版；作者提供含修订的 PDF | 免费教材＋作者课件＋官网链接的暑期课录像/练习 | 较新的系统教材；录像年份未逐项确认，按章节主题对应 |
| [CS276](https://web.stanford.edu/class/cs276/) / [IIR](https://nlp.stanford.edu/IR-book/) | 2019 课程存档＋2008 经典教材 | 公开 slides 与书籍 | 经典 IR 基础；现代神经检索结合专题教程 |
| [Retrieve & Re-Rank](https://sbert.net/examples/sentence_transformer/applications/retrieve_rerank/README.html) | 当前维护的官方教程 | 文档与例子，无必需视频 | 为经典 IR 增补现代检索/重排流程；实践时记录包版本 |
| [CSE258](https://cseweb.ucsd.edu/classes/fa25/cse258-a/) / [PML](https://cseweb.ucsd.edu/~jmcauley/pml/) | Fall 2025 课程＋2022 教材/作者 draft | 作者 PDF 为稳定主入口；课件/notebook 外链权限未全查 | 章节映射参考[作者教学页](https://cseweb.ucsd.edu/~jmcauley/)列出的 CSE258 fa25 |
| [Google Recommendation Systems](https://developers.google.com/machine-learning/recommendation) | 当前官方课程网页，无固定年版承诺 | 文字课程补充 | 连接候选生成、打分、重排 |
| [HF Agents Course](https://huggingface.co/learn/agents-course/en/unit0/introduction) | 当前持续维护的课程 | Unit 1/2/3＋evaluation bonus；使用当前页面 | 更新快的 Agent 工具用当前官方内容，实际运行记录框架版本 |
| [CS336](https://cs336.stanford.edu/) | Spring 2026 | 官网公开材料和录像列表入口；逐视频播放核查未完成 | 第 15 讲 SFT/RLHF、第 16 讲 RLVR；第 17 讲多模态选读。按 2026 目录定位讲次 |
| [IBM Variational Algorithm Design](https://quantum.cloud.ibm.com/learning/en/courses/variational-algorithm-design) | 当前官方课程页面 | 课程文字为主；API 以实际 SDK 版本为准 | 学习变分工作流，通过基线比较评价性能 |
| [Qiskit transpilation](https://quantum.cloud.ibm.com/docs/en/guides/transpile) | 当前官方文档 | 文档为主，无指定历史 SDK 视频 | 编译 API 和硬件接口随版本变化，开始实验时锁定版本 |
| [D-Wave models](https://docs.dwavequantum.com/en/latest/concepts/models.html) / [OR-Tools](https://developers.google.com/optimization) | 当前官方技术文档 | 建模与求解参考 | 先学表示与经典基线，再评价量子方法；固定依赖版本 |
| [RL for Quantum Technology](https://arxiv.org/abs/2601.18953) | 2026 综述，交叉导读入口 | 综述＋原始论文；无统一配套课程视频 | 提供近期研究地图，论点回原论文核实 |

## 视频筛选规则

1. 采用授课教师、大学或课程官网直接链接的录像。
2. 基础课可以保留经典年份；快速变化的课先核对最新版 syllabus，再确认该版公开视频是否存在。
3. 找到较新课件但没有确认同年完整录像时，直接说明；可先读新课件，旧录像只解释稳定概念。
4. 教材版次、课件年份、视频年份分别记。上传日期不自动等于录制日期。
5. 开始实际学习前再核查一次对应课程；更新影响章节安排时记录版本与差异。

## 新材料入选时必须填写

- 课程/材料名与官方链接。
- 完整核心知识地图；本计划选学部分单独标记。
- 经典基础 / 新版课程 / 当前官方文档 / 原始论文中的哪一类，以及选择理由。
- 作者、出版/授课年份、版次或版本号、核查日期。
- 文字、视频和代码各自可用性，以及它们是否同版。
- 对应的知识主题、先修关系与阅读范围。
