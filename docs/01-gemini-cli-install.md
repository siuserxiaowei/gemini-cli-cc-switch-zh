# Gemini CLI 安装（中国环境）

配套站内长文（含截图与更新记录）：[Gemini CLI 中国安装教程](https://nano-banana.lol/tutorials/gemini-cli-install-china)。

## 安装前

1. 确认 Node.js 版本满足官方当前要求（以官方 README / `engines` 字段为准）。
2. 不要混用多个全局包管理器反复覆盖同一命令名。
3. 安装脚本与包只从官方或你已核验的 registry 拉取。

## 常见装法（概念）

| 方式 | 注意 |
| --- | --- |
| 官方推荐的 npm / 安装器 | 装完执行 `gemini --version`（或以官方实际命令名为准） |
| 版本管理器（nvm / fnm 等） | 确认 `which gemini` 指向当前 shell 的 Node 前缀 |
| 多来源冲突 | 同一机器上旧全局包会抢 PATH |

## 登录前检查

- 明确你用的是 **Google 账号登录** 还是 **API Key / 其他 provider**——额度和账单互不相通。
- 不要在 Issue 或群聊粘贴完整 Key。
- 若下一步要走代理，先读 [代理篇](02-gemini-cli-proxy.md)，再登录，避免「登录成功但请求全挂」。

## 装好后最小验证

```bash
# 命令名以你安装的包为准
gemini --help
gemini --version
```

若 `command not found`：检查 PATH、是否装到了另一个 Node 前缀、是否需要新开终端。

下一步：[代理排错](02-gemini-cli-proxy.md) · 站内教程 <https://nano-banana.lol/tutorials/gemini-cli-install-china>
