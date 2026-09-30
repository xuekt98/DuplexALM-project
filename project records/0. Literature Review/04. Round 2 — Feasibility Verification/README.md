# Round 2 Brainstorm 方向可行性核查（深度）

> ARS `deep-research` `lit-review` 模式
> 流程：50 个精准关键词核查 Round 2 新的 5 个方向

## 文件清单

1. **`01. Verification Report — Round 2 Brainstorm Directions.md`** — 综合核查报告

## 数据基础

- 50 个精准查询 / 585 篇去重论文
- 严格 title-filter：标题必须包含相关术语

## 一句话结论

| Rank | 方向 | 严格筛选 | 综合判断 |
|---|---|---|---|
| ★★★★★ 1 | **T1 Audio Data Curation Agent** | **0 strict hits（真空）** | **首选** |
| ★★★★ 2 | **T4 Audio-Dependency Verification** | 3 strict hits | 推荐 |
| ★★★★ 3 | **T2 Audio Editing Agent** | 4 strict hits | 推荐 |
| ★★★ 4 | **T5 Smart Glasses First-Person Audio Agent** | 6 strict hits | 有条件推荐 |
| ★★ 5 | **T3 SFX AIGC Pipeline** | 21 strict hits | **降级**（已饱和）|

## 关键发现

- **T1 是真正真空**：没有任何论文做 "audio data curation via LALM agent"
- **T3 已被深度开路**：21 篇 Foley / SFX generation 工作（HunyuanVideo-Foley, FoleyDesigner 等）
- **T4 已有 3 篇前期工作**（Do Audio LMs Use Paralinguistic Evidence 等）但未饱和
- **T2 部分开路**：4 strict hits（video editing 为主），audio editing + agent 仍有 niche
- **T5 部分开路**：6 strict hits（egocentric 已有），agent 仍 niche

## 关键判断

- **首选 T1 Audio Data Curation Agent**：综合最优（真空 + 痛点真实 + AIGC 经验匹配 + 与团队都有接口）
- **不推荐 T3 SFX AIGC Pipeline**：与 HunyuanVideo-Foley / FoleyDesigner 等正面竞争
- **早期 niche (T2, T4, T5)**：可补充完整 framework
