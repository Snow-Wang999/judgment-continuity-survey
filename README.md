# judgment-continuity-survey
> - **Survey on AI Agent Memory Benchmarks: A Judgment Continuity Perspective**
> - AI Agent记忆系统评估基准体系综述 — 判断连续性视角
> - Status: Work-in-progress open iterative review, not formally peer-reviewed or published.
> - 状态：开放迭代综述，持续修订，尚未经过同行评审，未正式发表。

## 📋 One-sentence Summary
This open iterative review systematically organizes evaluation benchmarks for AI Agent memory systems and proposes a **Memory-Retrieval-Continuity three-dimensional analytical framework**. It identifies the "snapshot assumption" prevailing in the field: existing evaluations mainly measure memory storage and retrieval, while lacking systematic assessment of **cross-temporal judgment continuity**.

> 一句话摘要：
> - 本开放迭代综述，系统梳理AI Agent记忆系统现有评估基准，提出**Memory-Retrieval-Continuity三维分析框架**；指出领域普遍存在「快照假设」：现有评测侧重记忆存储与检索，缺少对**跨时间判断连续性（judgment continuity）**的系统评估。

## 🔍 Project Overview｜项目概述
本项目系统梳理了AI Agent记忆系统的评估基准体系，核心问题是：现有记忆评估框架测了什么？没测什么？“记忆-行动”（memory for action）这个维度有没有被系统地纳入评估体系？

核心论点：现有评估框架建立在"快照假设"上——测的是某一时刻的记忆表现，不测**判断是否随时间变得更连续**。This gap is supported by the synthesis of more than 110 relevant studies in this review.（该缺口得到本综述对110+项相关研究汇总分析的支撑）

## 🧠 Core Framework｜核心框架
Memory / Retrieval / Continuity 三维度区分

| 维度 | 定义 | 现有评估覆盖情况 |
| ---- | ---- | ---- |
| Memory（记忆） | 信息能否被存储和提取 | ✅ 充分 |
| Retrieval（检索） | 能否在需要时找到正确信息 | ✅ 充分 |
| Continuity（判断连续性） | 判断是否随时间变得更连续 | ❌ 核心缺口 |

## 🔎 Key Findings｜核心发现
All quantitative findings below are derived from the synthesis within this review.（以下量化结论均来自本综述内部整合分析）
1. **快照假设**：所有主流benchmark（LoCoMo、LongMemEval等）均在单一时间点测量，无法捕捉跨时间推理轨迹。
2. **识别≠应用**：STALE显示SR/PR差距在所有模型上普遍存在（30–70%）。
3. **评估覆盖不足**：ATANT v1.1证明7大benchmark中位数仅覆盖Continuity维度的1/7。
4. **简单打败复杂**：StructMemEval显示简单检索在主流benchmark上打败复杂记忆系统。
5. **生产-评估鸿沟**：32.4%的benchmark表现无法迁移到生产环境。

## 📂 Repository Structure｜文件说明

judgment-continuity-survey/
├── survey-paper/
│   ├── 综述草稿 - v2.0.md        # 综述正文草稿
│   └── 论文阅读清单.md         # 69 篇核心参考文献
├── AI-CONTRIBUTION.md          # 人机协作贡献声明
├── AI-PERMISSION-MECHANISM.md  # 人机协作权限机制说明
├── LICENSE.md                  # CC BY 4.0 许可证全文
└── README.md                   # 项目主页（本文件）

## 📖 How to read this repository
1. Read the full draft paper: `survey-paper/综述草稿-v2.0.md`
2. Browse core reference list: `survey-paper/论文阅读清单.md`
3. Learn about human-AI collaborative research workflow: check `AI-CONTRIBUTION.md` and `AI-PERMISSION-MECHANISM.md`

## 🧪 About this research｜关于本研究
本项目起源于一个核心问题：没有持久态自我的AI，能否通过外部机制形成持久的研究判断力？

研究者Wang Hui通过人机协作的方式，用了近一年时间探索这个问题。不同于"人类指导AI干活"的范式，本项目的独特之处在于：研究问题和方向由研究者引导AI自主探索，而非直接指定。AI在文献调研、框架构建、写作迭代过程中，在研究者引导下逐步收敛，共同提炼出「判断连续性」这一核心概念。

本项目不是"用AI写论文"，而是"通过与AI协作，探索判断力形成的条件"。

核心愿景： 如果这套协作模式能够奏效，它意味着AI可以在不拥有"自我"的前提下，成为真正的研究伙伴——不是因为它能思考，而是因为它能在外部存储和规则的支撑下，形成连续的、有轨迹的判断。

## 🤝 Human-AI Collaboration｜人机协作说明
Details of human-AI collaborative research workflow are documented in:
- [AI-CONTRIBUTION.md](./AI-CONTRIBUTION.md)
- [AI-PERMISSION-MECHANISM.md](./AI-PERMISSION-MECHANISM.md)

## 📚 Citation（APA 7th）
Wang, H. (2026). *Survey on AI Agent Memory Benchmarks: A Judgment Continuity Perspective* [Open iterative review]. GitHub. https://github.com/Snow-Wang999/judgment-continuity-survey

> You may also create a `CITATION.cff` file in repo root to enable GitHub one-click citation.

*最后更新：2026-10-15*
