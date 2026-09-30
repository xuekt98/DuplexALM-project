# FullDuplexLLM

全双工大模型方向研究项目：探索支持同时听与说、低延迟、可打断的全双工语音对话系统，包括流式 ASR、TTS、双工语音-语言联合建模等子方向。

> Initialized by the `mine-init-codex-project` skill on 2026-09-07.
> Edit this file to describe your project's structure, conventions, and any
> durable team agreements Codex should follow when working in this repo.

## Project Handbook

项目根目录下的 `project handbook/` 是 Codex 在每个新会话开始时默认读取的项目手册。**Codex 在开始任何工作前，都应自动加载以下文件：**

- `project handbook/project architecture/ARCHITECTURE.md` — 项目的组织架构、目录划分、模块边界与依赖关系。
- `project handbook/project rules/RULES.md` — 项目级操作规则，包含 Windows / PowerShell 路径安全禁令。
- `project handbook/project skills/` — 项目本地 skills 的存放目录；按需读取其中的 skill 文件。
- `project handbook/project tools/` — 仅在根据本项目需要定制的 tools 存放目录；按需读取使用。

**危险命令**：Windows / PowerShell 环境下不要用 `cmd /c` 做路径操作，要用 PowerShell 原生命令 + `-LiteralPath` + 单引号包裹路径，详见 `project handbook/project rules/RULES.md` “危险命令禁令” 一节。

临时文件统一放在仓库根目录下的 `codex temp/`（已在 `.gitignore` 中忽略其内容）。

## 项目结构

<!-- TODO: 用一两段说明仓库的目录划分与各子模块的用途。详细架构请写到 `project handbook/project architecture/ARCHITECTURE.md`。 -->

## 使用约定

<!-- TODO: 列几条本项目特有的约定，例如：构建命令、测试入口、提交前自检、依赖管理等。操作约束与危险命令禁令请写到 `project handbook/project rules/RULES.md`。 -->
