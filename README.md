# Gemini CLI / CC Switch 中文手册（安装 · 代理 · 供应商切换）

面向中文开发者：Google **Gemini CLI** 怎么装、国内代理怎么排，以及用 **CC Switch** 在 Claude Code / Codex / Gemini CLI 之间切换供应商。

> 非官方文档，与 Google、Anthropic、OpenAI 无隶属关系。命令随客户端版本变化，**以本机 `--help` 与官方文档为准**。最后整理：2026-11-03（Asia/Shanghai）。
>
> 本仓库是 [codex-claude-code-zh](https://github.com/siuserxiaowei/codex-claude-code-zh) 的**主题配套**（Gemini / 切换器），不是同一份 Codex/Claude 排错手册的拷贝。

## 目录

| 文档 | 解决什么问题 |
| --- | --- |
| [Gemini CLI 安装（中国环境）](docs/01-gemini-cli-install.md) | npm、版本核对、登录前检查 |
| [Gemini CLI 代理与 fetch failed](docs/02-gemini-cli-proxy.md) | HTTPS_PROXY、地区提示、断流 |
| [CC Switch：多 CLI 供应商切换](docs/03-cc-switch.md) | Claude Code / Codex / Gemini 之间切换 |
| [安全底线与脱敏问题单](docs/04-safety-checklist.md) | 不能贴什么、提问前先抄什么 |
| [和 Codex/Claude 手册怎么配合](docs/05-related-codex-claude.md) | 何时回链 codex-claude-code-zh |

## 30 秒分流

| 你看到的 | 先去 |
| --- | --- |
| `gemini: command not found` / 装不上 | [安装](docs/01-gemini-cli-install.md) |
| `fetch failed` / 超时 / 地区提示 | [代理](docs/02-gemini-cli-proxy.md) |
| 想在多个 Coding CLI 间换 Key / 端点 | [CC Switch](docs/03-cc-switch.md) |
| Codex / Claude 的 401·429 | 去配套仓 [codex-claude-code-zh](https://github.com/siuserxiaowei/codex-claude-code-zh) |

## Nano Banana 延伸阅读（本仓库只链本站）

- [Gemini CLI 中国安装教程](https://nano-banana.lol/tutorials/gemini-cli-install-china)
- [Gemini CLI 国内代理](https://nano-banana.lol/how-to/gemini-cli-proxy-china)
- [CC Switch 教程](https://nano-banana.lol/tutorials/cc-switch-codex-claude)
- [Gemini / Google AI 购买前核验](https://nano-banana.lol/gemini-pro)

## 许可

文字内容采用 [CC BY 4.0](LICENSE)。
