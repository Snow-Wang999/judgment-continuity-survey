# judgment-continuity-survey

**AI Agent记忆系统评估基准体系综述 — 判断连续性视角**

Survey on AI Agent Memory Benchmarks: A Judgment Continuity Perspective

---

## 项目概述

本项目系统梳理了AI Agent记忆系统的评估基准体系，核心问题是：现有记忆评估框架测了什么？没测什么？"记忆-行动"（memory for action）这个维度有没有被系统地纳入评估体系？

**核心论点：** 现有评估框架建立在"快照假设"上——测的是某一时刻的记忆表现，不测"判断是否随时间变得更连续"。这一缺口被110+项独立研究反复验证。

---

## 核心框架

**Memory / Retrieval / Continuity 三维度区分**

| 维度 | 定义 | 现有评估覆盖 |
|------|------|-------------|
| Memory（记忆） | 信息能否被存储和提取 | ✅ 充分 |
| Retrieval（检索） | 能否在需要时找到正确信息 | ✅ 充分 |
| Continuity（判断连续性） | 判断是否随时间变得更连续 | ❌ **核心缺口** |

---

## 核心发现

1. **快照假设**：所有主流benchmark（LoCoMo、LongMemEval等）均在单一时间点测量，无法捕捉跨时间推理轨迹
2. **识别≠应用**：STALE显示SR/PR差距在所有模型上普遍存在（30-70%）
3. **评估覆盖不足**：ATANT v1.1证明7大benchmark中位数仅覆盖Continuity维度的1/7
4. **简单打败复杂**：StructMemEval显示简单检索在主流benchmark上打败复杂记忆系统
5. **生产-评估鸿沟**：32.4%的benchmark表现无法迁移到生产环境

---

## 文件说明

| 文件 | 说明 |
|------|------|
| `survey-paper/综述草稿-v2.0.md` | 综述正文草稿 |
| `survey-paper/论文阅读清单.md` | 参考文献清单（69篇核心） |

---

## 综述主题

> **《AI Agent记忆系统的评估基准体系：现有框架评什么、缺什么》**

---

*最后更新：2026-10-15*
