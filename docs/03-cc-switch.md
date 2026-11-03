# CC Switch：在 Claude Code、Codex 与 Gemini CLI 之间切换供应商

配套：[CC Switch 教程](https://nano-banana.lol/tutorials/cc-switch-codex-claude)。

## 它解决什么

你同时维护多套 Coding CLI（Claude Code、Codex、Gemini CLI）时，经常要改：

- API Base / 供应商端点
- API Key 或登录态
- 默认模型名

CC Switch 类工具把「切换供应商」收成可重复的步骤，减少手改配置文件出错。

## 使用前原则

1. **备份**现有 `settings.json` / 环境变量导出（不要提交到公开仓库）。
2. 切换后先跑**只读**命令（`--help` / 列模型），再跑会耗额度的任务。
3. 确认当前 shell 没有残留的旧 `ANTHROPIC_*` / `OPENAI_*` / `GOOGLE_*` 变量互相覆盖。

## 典型流程（概念）

1. 安装并打开 CC Switch（以该项目当前 README 为准）。
2. 为每个供应商建一份配置档（命名清楚：`work-openai` / `home-gemini`）。
3. 切换后在对应 CLI 内验证身份路径（账号登录 vs Key）。
4. 出问题先看：是否切错档、Key 是否过期、代理是否仅对某一个域名生效。

## 和本站其他教程

- Gemini 装不上 → [安装](01-gemini-cli-install.md)
- Gemini 网络错误 → [代理](02-gemini-cli-proxy.md)
- Codex / Claude 401·429 → [codex-claude-code-zh](https://github.com/siuserxiaowei/codex-claude-code-zh)

站内完整图文：<https://nano-banana.lol/tutorials/cc-switch-codex-claude>
