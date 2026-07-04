<p align="center">
  <a href="https://github.com/Menfre01/waveloom/releases/latest"><img src="https://img.shields.io/github/v/release/Menfre01/waveloom?style=flat-square&color=00ADD8&labelColor=161b22" alt="release"/></a>
  <a href="https://github.com/Menfre01/waveloom/actions/workflows/ci.yml"><img src="https://github.com/Menfre01/waveloom/actions/workflows/ci.yml/badge.svg?style=flat-square&labelColor=161b22" alt="CI"/></a>
  <a href="https://go.dev"><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white&labelColor=161b22" alt="Go"/></a>
  <a href="https://platform.deepseek.com"><img src="https://img.shields.io/badge/DeepSeek-4D6BFE?style=flat-square&labelColor=161b22" alt="DeepSeek"/></a>
</p>

## 👋 你好，我是 Menfre

正在构建 **[Waveloom](https://github.com/Menfre01/waveloom)** — 一款**专为 DeepSeek 前缀缓存优化**的终端 Code Agent。体验对标 Claude Code，运行成本仅为其零头。

> Building **[Waveloom](https://github.com/Menfre01/waveloom)** — a terminal Code Agent purpose-built for DeepSeek prefix caching. Feels like Claude Code, costs a fraction to run.

### 为什么是 Waveloom？ / Why Waveloom?

DeepSeek 对缓存未命中的收费是命中的 **120 倍**。Waveloom 在架构层面保持 System Prompt 和消息前缀稳定 — 最长公共前缀在每一轮对话中都保持缓存热度。用 DeepSeek 的价格，获得 Claude Code 级别的 Agent 体验。

> DeepSeek charges up to 120× more for cache misses than hits. Waveloom keeps the prefix stable at the architecture level so the longest common prefix stays cache-hot across every turn.

| | Waveloom | Claude Code |
|---|---|---|
| 缓存设计 / Cache | 前缀稳定：固定 System Prompt、仅追加、原地压缩 | 动态分段，摘要替换消息 |
| 运行时 / Runtime | 单二进制 ~18MB | Node.js |
| Skills | 兼容 Claude Code Skills | 原生 |

**一行安装 / curl one-liner：**

```sh
curl -fsSL https://raw.githubusercontent.com/Menfre01/waveloom/main/install.sh | sh
```

```sh
waveloom setup
waveloom
```

### 核心特性 / Highlights

- **前缀缓存优化** — 固定 System Prompt，仅追加历史，四级水位线压缩。最长公共前缀跨轮次保持热度
- **权限安全** — 三级决策（允许 / 拒绝 / 询问）+ 模式匹配规则引擎，每次写入都需要确认
- **会话持久化** — `waveloom --continue` 随时恢复，完整上下文不丢失
- **Plan 模式** — 先探索设计、审批后再动手。前缀缓存安全的消息配对机制
- **9 个内置工具** — `read_file` / `write_file` / `edit_file` / `shell` / `web_fetch` / `skill` / …
- **完整双语** — 中英文 UI 切换，`/locale` 命令，自动检测系统语言
- **TUI 交互** — Bubble Tea + Glamour Markdown + Lipgloss，`@` 模糊文件选择器，`/` 命令面板

### 技术栈 / Tech Stack

Go · Bubble Tea · DeepSeek API · OpenAI API · LLM Agent · 61k+ 行

### 项目 / Projects

- **[waveloom](https://github.com/Menfre01/waveloom)** — 终端 AI 编码代理
- **[homebrew-tap](https://github.com/Menfre01/homebrew-tap)** — Homebrew 分发

### 找到我 / Find Me

- GitHub: [@Menfre01](https://github.com/Menfre01)
