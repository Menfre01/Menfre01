<p align="center">
  <a href="https://github.com/Menfre01/waveloom/releases/latest"><img src="https://img.shields.io/github/v/release/Menfre01/waveloom?style=flat-square&color=00ADD8&labelColor=161b22" alt="release"/></a>
  <a href="https://github.com/Menfre01/waveloom/actions/workflows/ci.yml"><img src="https://github.com/Menfre01/waveloom/actions/workflows/ci.yml/badge.svg?style=flat-square&labelColor=161b22" alt="CI"/></a>
  <a href="https://go.dev"><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white&labelColor=161b22" alt="Go"/></a>
</p>

## 👋 你好，我是 Menfre

后端/基础设施方向的开发者，目前在用 Go 折腾 LLM Agent 相关的东西。喜欢把复杂问题拆成干净的 API，追求零依赖、单二进制、能跑十年的代码。

> Backend / infra engineer building LLM agents in Go. I like clean APIs, zero-dependency binaries, and code that still runs ten years later.

### 🛠️ 技术栈

Go · Bubble Tea · DeepSeek API · OpenAI API · LLM Agent · TUI

### 📦 作品

**[Waveloom](https://github.com/Menfre01/waveloom)** — 专为 DeepSeek 前缀缓存优化的终端 Code Agent

DeepSeek 缓存命中与未命中的价差高达 120 倍。Waveloom 在架构层面保持前缀稳定，用 DeepSeek 的价格跑出 Claude Code 的体验。61k+ 行 Go，单二进制 ~18MB，curl 一行安装。

> A terminal Code Agent purpose-built for DeepSeek prefix caching. Prefix-stable architecture keeps the longest common prefix cache-hot — Claude Code–level experience at a fraction of the cost.

核心特性：前缀缓存优化 · 权限安全 · 会话持久化 · Plan 模式 · 9 个内置工具 · 完整中英双语 · Bubble Tea TUI

```sh
curl -fsSL https://raw.githubusercontent.com/Menfre01/waveloom/main/install.sh | sh
```

**[homebrew-tap](https://github.com/Menfre01/homebrew-tap)** — Waveloom 的 Homebrew 分发配方

### 🔗 找到我

- GitHub: [@Menfre01](https://github.com/Menfre01)
