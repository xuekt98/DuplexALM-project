# Audio Frontier & Audio-Visual Research 2026

> 第二轮 ARS `lit-review` 输出。本轮覆盖范围：**音频前沿（不止 duplex）+ 音视觉结合**，时间窗口 **arXiv 2026-01 至 2026-09**。

## 阅读顺序建议

1. **`00. Overview — Audio Frontier & Audio-Visual 2026.md`** — 全局图景：8 大主题、关键观察、与 FullDuplexLLM 项目的对应表、检索方法与可复现性。
2. **`01. Audio Frontier Research Directions 2026.md`** — 8 大音频前沿方向（音频 LLM 推理化、音乐、TTS/克隆、ASR、对话、空间、推理、安全）的深度展开。
3. **`02. Audio-Visual Research 2026.md`** — **本轮 review 重点**：音视觉 9 篇核心论文的感知 / 生成 / 安全 / 评测四象限分析。
4. **`03. 2026 arxiv Reading List.md`** — 63 篇精炼论文的 annotated bibliography，每条记录附 arXiv ID + 摘要 + 与 FullDuplexLLM 相关度。
5. **`04. 2026 Challenges & Benchmarks Catalog.md`** — 25 个 2026 audio challenge / benchmark 的目录与时间表。

## 数据文件 (`raw/`)

| 文件 | 内容 |
|---|---|
| `raw/_consolidated.json` | 80 篇原始检索记录（去重后） |
| `raw/_consolidated_2026.json` | 72 篇 2026-only 论文 |
| `raw/_relevant.json` | 63 篇强相关论文（最终入选） |
| `raw/_themes.json` | 按 14 个主题分桶的论文 |
| `raw/*.txt` | 各次 arXiv API 查询的原始输出 |

## 与已有项目记录的关系

- 项目已有 `0. Literature Review/`（首轮 overview，**仅限 Full-Duplex Audio LLM**）
- 本轮 `1. Audio Frontier & Audio-Visual 2026/` 是第二轮，**范围更广**，与首轮互补不重复
- 后续可考虑：
  - `2. Survey of XX/` — 后续具体方向细读
  - 把某些强相关论文（如 VISA, Seedance 2.0, Audio-DeepThinker）补充到 `0. Literature Review/01. Reading List — Full-Duplex Audio LLM.md`

## 关键论文（按相关度排序）

### 与 FullDuplexLLM 紧密相关（★★★）

1. **VISA** (2606.07264v2) — 视觉证据辅助音频推理的 agentic 范式
2. **Separate First, Then Associate** (2608.14812) — 真实场景下 AVSE
3. **Audio-DeepThinker** (2604.18187) — Progressive Reasoning-Aware RL for LALM CoT
4. **Audio-Cogito** (2604.12527v3) — 开源 LALM 推理
5. **ICASSP 2026 HumDial Challenge** (2601.05564v2) — Human-like Spoken Dialogue 系统评测标准
6. **HumDial-EIBench** (2604.11594v2) — ALM emotional intelligence 评测
7. **SLT 2026 SmartGlasses Challenge** (2608.12034) — 第一视角多说话人识别
8. **Interspeech 2026 ARC** (2602.14224) — Audio Reasoning Challenge with MMAR Rubrics

### 音视觉重点（★★）

9. **Seedance 2.0** (2604.14148) — 字节原生多模态音视频生成
10. **AIGC Audio-Video Detection** (2607.25543) — Modality-Decoupling 颠覆性发现
11. **POLY-SIM 2026** (2603.24569v2, 2607.13669) — 多语言多模态说话人 ID
12. **GENEA Challenge 2026** (2608.10839) — 共语音手势生成
13. **Super Star** (2608.24909) — 流式实时手势生成
14. **Multi2AV-Safety** (2608.26535) — 多模态→音视频安全
15. **ABAW11 A/H** (2607.15779v2) — Ambivalence/Hesitancy 识别
16. **V-SONAR** (2603.01096) — 多语言多模态嵌入空间

## 局限性

- 仅检索 arXiv，未覆盖 ICASSP / Interspeech / ACL 已接收但未挂 arXiv 的论文
- 部分论文版本号 v1–v5 以 v1 为锚定，未来 v2+ 可能替换
- 未做单篇 citation verification（per ARS Iron Rule，下游 paper-writing 阶段需补 S2/OpenAlex/Crossref 校验）
- 关键词命中偏差：用 `abs:"<keyword>"` 检索，可能漏掉同义词表达
