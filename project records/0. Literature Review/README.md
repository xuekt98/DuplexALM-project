# 0. Literature Review — FullDuplexLLM Project

> 本目录是 FullDuplexLLM 项目的**所有文献调研、研究方向思考、可行性核查**的归档。
> 按**时间线 + 工作流**组织，每个子目录代表一轮独立的迭代，每一轮都引用前一轮。

---

## 📁 目录结构

```
0. Literature Review/
├── 00. Initial Review — Full-Duplex Audio LLM/        ← 项目初始文献综述（Full-Duplex Audio LLM 范围）
├── 01. Round 1 — Audio Frontier & Audio-Visual 2026/ ← 第 1 轮：扩展到 audio 前沿 + 音视觉结合
├── 02. Brainstorming — From AIGC to Audio/            ← 第 2 轮：基于 lit-review 产生 brainstorm 方向
├── 03. Round 1 — Feasibility Verification/           ← 第 3 轮：核查 Round 1 brainstorm 是否可行
└── 04. Round 2 — Feasibility Verification/           ← 第 4 轮：核查 Round 2 brainstorm 是否可行
```

---

## 🔄 工作流时间线

| 阶段 | 子目录 | 输入 | 输出 |
|---|---|---|---|
| **00 初始** | `00. Initial Review` | 项目立项 | **Full-Duplex Audio LLM** 全景概览（4 篇综述/reading list）|
| **01 第 1 轮 lit-review** | `01. Round 1` | 初始 overview + 用户要求扩展 | 2026 audio 前沿 + 音视觉结合 的 5 份报告 + 65 篇精炼论文 |
| **02 Brainstorming** | `02. Brainstorming` | Round 1 lit-review 发现 | AIGC → audio 跨界的 18 个候选方向 + Top 5 推荐 |
| **03 第 1 轮 verification** | `03. Round 1` | Round 1 brainstorm Top 5 | 验证可行性 + 发现 audio editing 不是真空 |
| **04 第 2 轮 verification** | `04. Round 2` | Round 2 brainstorm Top 5 | 深度核查 50 个关键词，确认 T1 Audio Data Curation Agent 是真真空 |

**核心循环**：lit-review → brainstorm → verification → re-brainstorm → re-verify

---

## 📚 详细文件清单

### 00. Initial Review — Full-Duplex Audio LLM
项目初始的全双工音频大模型文献综述（项目立项时的 baseline）。

| 文件 | 内容 |
|---|---|
| `00. Overview — Full-Duplex Audio LLM.md` | 初始 overview（7 主线 + 关键观察）|
| `01. Reading List — Full-Duplex Audio LLM.md` | 按重要性排序的精读清单（A. 综述 / B. 奠基 / C. 突破期 / D. 工业落地 等）|
| `02. 2026 Survey List — Full-Duplex Audio LLM.md` | 2026 年相关 survey 清单（ICMI 2026 / HumDial / SLT 2026 等）|
| `03. Audio Preprocessing & Tokenization Pipeline — Technical Reference.md` | 音频编解码 / tokenization 技术参考 |

### 01. Round 1 — Audio Frontier & Audio-Visual 2026
**第 1 轮 lit-review**：从 Full-Duplex Audio LLM 扩展到 audio 前沿 + 音视觉结合。
**检索**：arXiv 2026-01 至 2026-09，~45 个关键词 / 80 篇去重 / 65 篇强相关。

| 文件 | 内容 |
|---|---|
| `00. Overview — Audio Frontier & Audio-Visual 2026.md` | 第 1 轮 overview（9 主线 + 关键观察）|
| `01. Audio Frontier Research Directions 2026.md` | 8 大音频前沿方向（Audio LLM / Music / TTS / ASR / 对话 / 空间 / 推理 / 安全）|
| `02. Audio-Visual Research 2026.md` | 音视觉结合深度（感知 / 生成 / 安全 / 评测四象限）|
| `03. 2026 arxiv Reading List.md` | 65 篇精炼论文的 annotated bibliography |
| `04. 2026 Challenges & Benchmarks Catalog.md` | 26 个 2026 audio challenge / benchmark |
| `raw/` | 75 份 arXiv API 原始查询记录 + consolidated JSON |

### 02. Brainstorming — From AIGC to Audio
**第 2 轮 brainstorm**：基于 Round 1 lit-review，思考 AIGC → audio 跨界的研究方向。

| 文件 | 内容 |
|---|---|
| `01. Brainstorming Candidates — Raw Pool.md` | 18 个原始候选（AIGC 迁移 + 跨界 + 痛点 + 基础设施 + 安全）|
| `02. Brainstorming Filtered & Ranked.md` | Round 1 Top 5 + 备选 5 + 决策矩阵 |
| `03. Re-Brainstorm Round 2 — Niche Cross & Engineering Differentiation.md` | Round 2 brainstorm（修正策略：从"找空白"到"niche 交叉 + 工程差异化"），20 个候选 + 新 Top 5 |
| `README.md` | brainstorm 流程说明 |

### 03. Round 1 — Feasibility Verification
**第 3 轮 verification**：核查 Round 1 brainstorm 的 10 个方向可行性。
**检索**：~80 个关键词 / 1586 篇去重论文 / 严格 title-filter。

| 文件 | 内容 |
|---|---|
| `01. Verification Methodology and Key Findings.md` | 第 1 轮核查方法 + 关键发现（FM era audit）|
| `02. Final Verified Top 5 Recommendations.md` | 修正版 Top 5 |
| `03. REVISED — Traditional Audio Editing Exists.md` | 用户驱动修正：audio editing 不是真空（245 篇相关）|
| `04. Comprehensive Verification of ALL 10 Directions.md` | 完整 10 方向核查 + 重新排序 |
| `raw/` | 185 份 arXiv API 原始查询记录 + consolidated JSON |

### 04. Round 2 — Feasibility Verification
**第 4 轮 verification**：核查 Round 2 brainstorm 的 5 个新方向可行性。
**检索**：50 个精准关键词 / 585 篇去重论文 / 严格 title-filter。

| 文件 | 内容 |
|---|---|
| `01. Verification Report — Round 2 Brainstorm Directions.md` | Round 2 深度核查报告 |
| `raw/` | 54 份 arXiv API 原始查询记录 + consolidated JSON |

---

## 🏆 最终推荐（基于全部 4 轮核查）

| Rank | 方向 | 严格筛选 | 状态 |
|---|---|---|---|
| ★★★★★ 1 | **T1 Audio Data Curation Agent** | 0 strict hits | **真空 niche，强烈推荐** |
| ★★★★ 2 | **T4 Audio-Dependency Verification** | 3 strict hits | niche 存在，推荐 |
| ★★★★ 3 | **T2 Audio Editing Agent** | 4 strict hits | 部分开路，推荐 |
| ★★★ 4 | **T5 Smart Glasses First-Person Audio Agent** | 6 strict hits | agent 仍 niche |
| ★★ 5 | **T3 SFX AIGC Pipeline** | 21 strict hits | **已被开路，不推荐** |

**首选方向**：T1 Audio Data Curation Agent —— 真空 niche + 痛点真实 + AIGC 经验匹配。

---

## 📖 推荐阅读顺序

如果你想快速了解全貌：

1. **本 README**（5 分钟）
2. **`00. Initial Review/00. Overview — Full-Duplex Audio LLM.md`**（10 分钟）— 项目基线
3. **`01. Round 1/00. Overview — Audio Frontier & Audio-Visual 2026.md`**（15 分钟）— 第 1 轮全景
4. **`02. Brainstorming/03. Re-Brainstorm Round 2.md`**（20 分钟）— 修正后的 brainstorm
5. **`04. Round 2/01. Verification Report.md`**（15 分钟）— 最终核查结论

如果你想深挖某个方向：从 `02. Brainstorming/02. Brainstorming Filtered & Ranked.md` 找到对应方向的 two-sentence pitch，再到 `04. Round 2/01. Verification Report.md` 查该方向的 strict hits 列表。

---

## ⚠️ 局限性

- **arXiv only**：所有检索都基于 arXiv API（ToU 3 秒间隔），未覆盖 ICASSP / Interspeech / ACL 已接收但未挂 arXiv 的论文
- **未做单篇 citation verification**（per ARS Iron Rule）：本 lit-review 不做 S2 / OpenAlex / Crossref 三源校验；下游 paper-writing 阶段需补
- **版本锚定**：以 arXiv v1 为锚定，未来 v2+ 可能替换
- **关键词命中偏差**：用 `abs:"<keyword>"` 检索，可能漏掉同义词表达
- **数据时效性**：截至 2026-09-11，2026-09 后新论文未覆盖
