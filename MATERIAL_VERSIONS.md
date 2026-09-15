# 教材、课程与视频：版本档案

核查日期：**2026-09-15**。选材原则：经典基础建立长期框架；快速变化的方法、工具和后训练内容采用较新的官方材料。这里的“经典”是本计划对教学价值的判断，不是声称存在一个客观的“最经典”排名。

“当前官方页面”不等于所有内容均于 2026 更新；“官网提供视频入口”不等于已逐条验证可播放。以下把确认的信息与尚未确认的信息分开写。

## v3 当前使用范围

固定主资源仅为 D2L、Watrous、CS285、MARL Book、PML、HF Agents 六套。下表保留之前核查的来源档案，**不是全部需要学习的清单**。

CS229、Preskill、MML 暂不安排；Silver 只作 RL 缺口的替代解释；CS336 只在后训练具体概念不清楚时查询。CS276/CSE258 只查目录映射，不整课跟读。其他官方教程按 [课程指南](COURSES.md) 的五个短模块选节使用。年份和可用性判断保持原核查边界。

## 来源版本档案

| 材料 | 选用版本/类型 | 教材与视频安排 | 为什么选它 / 边界 |
|---|---|---|---|
| [D2L](https://d2l.ai/) | 成熟系统教材；官网当前标记 1.0.3 | 在线教材/代码为主；不额外拼接未核查的视频课 | 用统一框架串起模型与训练；不作为最新 LLM 后训练资料 |
| [CS229 notes](https://cs229.stanford.edu/main_notes.pdf) | PDF 标注 2026-08-23 | 选这版公开讲义；没有把旧视频自动配成同版 | 经典 ML 体系的较新讲义，补泛化、表示学习等理论 |
| [MML](https://mml-book.github.io/) | 2020 出版；作者在线 PDF/勘误入口 | 仅数学查阅，不作为额外主课 | 稳定基础不需要追逐年份；具体下载版本在开始查阅时记录 |
| [Watrous 系列统一讲义](https://arxiv.org/abs/2507.11536) | 2025 arXiv 公开讲义；IBM 当前课程页 | Basics / General Formulation / Algorithms / QEC 各自使用官网文字与配套视频入口 | 系统、较新且连贯；视频具体录制年未逐一确认，不称为“2026 新视频” |
| [Preskill Ph219](https://www.preskill.caltech.edu/ph219/) | 经典讲义，逐章更新 | QEC 第 7 章网页标为 2026-03；第 2–3 章为 2015；2020 录播仅对应第 1–6 章 | 经典理论补充，明确不以旧录像代替新版 QEC |
| [Silver RL](https://davidstarsilver.wordpress.com/teaching/) | 2015 经典公开课 | 使用作者官网提供的视频与 slides | MDP/TD/PG 的基础结构清楚；PPO/SAC/LLM RL 由后续课程补 |
| [Sutton & Barto](https://mitpress.mit.edu/9780262352703/reinforcement-learning/) | 第二版，2018，经典教材 | 作为定义与理论参考；视频由 Silver 承担 | 不把它当作最新 Deep RL 算法目录 |
| [CS285/185](https://rail.eecs.berkeley.edu/deeprlcourse/) | 官网当前为 Spring 2026 | **主用 2026 讲义**；官网列出的 2023 录播只用于重合基础主题的补充 | 新课件覆盖 LLM/offline/model-based RL；不声称 2023 是最新录播，讲次不混用 |
| [MARL Book](https://www.marl-book.com/) | 2024 出版；作者提供含修订的 PDF | 免费教材＋作者课件＋官网链接的暑期课录像/练习 | 较新的系统教材；录像年份未在本轮逐项确认，按章节主题对应 |
| [CS276](https://web.stanford.edu/class/cs276/) / [IIR](https://nlp.stanford.edu/IR-book/) | 2019 课程存档＋2008 经典教材 | 公开 slides / 书籍主修；不依赖 Canvas 视频 | 经典 IR 基础保留，不能覆盖现代神经检索全部进展 |
| [Retrieve & Re-Rank](https://sbert.net/examples/sentence_transformer/applications/retrieve_rerank/README.html) | 当前维护的官方教程 | 文档与例子，无必需视频 | 为经典 IR 增补现代检索/重排流程；实践时记录包版本 |
| [CSE258](https://cseweb.ucsd.edu/classes/fa25/cse258-a/) / [PML](https://cseweb.ucsd.edu/~jmcauley/pml/) | Fall 2025 课程＋2022 教材/作者 draft | 作者 PDF 为稳定主入口；课件/notebook 外链权限未全查 | [作者教学页](https://cseweb.ucsd.edu/~jmcauley/)本次列出的最近 CSE258 是 fa25；不泛称全网最新推荐课 |
| [Google Recommendation Systems](https://developers.google.com/machine-learning/recommendation) | 当前官方课程网页，无固定年版承诺 | 文字课程补充 | 连接候选生成、打分、重排；不替代完整推荐教材 |
| [HF Agents Course](https://huggingface.co/learn/agents-course/en/unit0/introduction) | 当前持续维护的课程 | Unit 1/2/3＋evaluation bonus；使用当前页面 | 更新快的 Agent 工具用当前官方内容，实际运行记录框架版本 |
| [CS336](https://cs336.stanford.edu/) | **Spring 2026，替换原计划的 2025 版** | 官网公开材料和录像列表入口；本次逐视频播放核查未完成 | 第 15 讲 SFT/RLHF、第 16 讲 RLVR；第 17 讲多模态选读。新旧讲次不同 |
| [IBM Variational Algorithm Design](https://quantum.cloud.ibm.com/learning/en/courses/variational-algorithm-design) | 当前官方课程页面 | 课程文字为主；API 以实际 SDK 版本为准 | 学变分工作流；不将课程营销表述当成量子优势证据 |
| [Qiskit transpilation](https://quantum.cloud.ibm.com/docs/en/guides/transpile) | 当前官方文档 | 文档为主，无指定历史 SDK 视频 | 编译 API 和硬件接口随版本变化，开始实验时锁定版本 |
| [D-Wave models](https://docs.dwavequantum.com/en/latest/concepts/models.html) / [OR-Tools](https://developers.google.com/optimization) | 当前官方技术文档 | 建模/求解模块，不伪装成一门完整课程 | 先学表示与经典基线，再评价量子方法；固定依赖版本 |
| [RL for Quantum Technology](https://arxiv.org/abs/2601.18953) | 2026 综述，交叉导读入口 | 综述＋原始论文；无统一配套课程视频 | 提供近期研究地图，论点回原论文核实 |

## 视频筛选规则

1. 首选授课教师、大学或课程官网直接链接的录像；不使用来源不明的剪辑合集作为主课。
2. 基础课可以保留经典年份；快速变化的课先核对最新版 syllabus，再确认该版公开视频是否存在。
3. 找到较新课件但没有确认同年完整录像时，直接说明；可先读新课件，旧录像只解释稳定概念。
4. 教材版次、课件年份、视频年份分别记。上传日期不自动等于录制日期。
5. 开始实际学习前再核查一次对应课程；更新影响章节安排时记录差异，不悄悄更换课程版本。

## 新材料入选时必须填写

- 课程/材料名与官方链接。
- 完整核心知识地图；本计划选学部分单独标记。
- 经典基础 / 新版课程 / 当前官方文档 / 原始论文中的哪一类，以及选择理由。
- 作者、出版/授课年份、版次或版本号、核查日期。
- 文字、视频和代码各自可用性，以及它们是否同版。
- 与已有主课程的重合和新增内容；不能仅因为“新”就加入第三条学习线。

此表不触发自动更新，也没有注册课程、下载教材全文或运行云计算任务。
