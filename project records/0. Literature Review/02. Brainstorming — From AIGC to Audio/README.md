# Research Ideation — From AIGC to Audio

> brainstorming-research-ideas skill 输出
> 上下文：用户从 AIGC 转 audio 方向；团队已有 duplex ALM + 音乐生成
> 流程：Diverge（15+ 候选）→ Converge（filter）→ Refine（Top 5 + two-sentence pitch）

## 文件清单

1. **`01. Brainstorming Candidates — Raw Pool.md`** — 18 个候选方向的原始池，按来源分类（AIGC 直接迁移 / 跨界融合 / audio 痛点 / 基础设施 / 安全反 AI）
2. **`02. Brainstorming Filtered & Ranked.md`** — Top 5 + 备选 5 + 优先级评分 + 2-Week Pilot 建议

## Top 5 一句话摘要

| # | 方向 | 优先级 | 核心 AIGC 迁移 |
|---|---|---|---|
| 1 | **Audio Latent Editing** | ★★★★★ | SD img2img / DragGAN 思路 → 音频版 |
| 2 | **Audio Watermarking for AIGC** | ★★★★☆ | Tree-Ring / Gaussian-Shading → 音频版 |
| 3 | **Streaming Audio Diffusion + Distillation** | ★★★★☆ | SD-Turbo / Consistency Models → 1-step 音频扩散 |
| 4 | **Audio Agentic System** | ★★★★☆ | text agent ReAct → 音频版 |
| 5 | **Audio Reasoning + AIGC Generation** | ★★★☆☆ | CoT 推理 + 多模态 token 生成 |

## 两条路径建议

- **路径 A（差异化优先）**：Top 1 + Top 2
- **路径 B（协同优先）**：Top 3 + Top 4

详见 `02. Brainstorming Filtered & Ranked.md`。
