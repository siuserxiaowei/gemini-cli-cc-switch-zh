# 安全底线与脱敏问题单

## 绝对不要发

- API Key、OAuth refresh token、`auth.json`、Cookie、Session
- 邮箱验证码、短信码、备份码
- 未打码的账单截图（卡号、完整邮箱+订单可联动的信息）

## 提问前请附上（脱敏后）

- [ ] 客户端名称与版本（`gemini --version` / 对应 CLI）
- [ ] 操作系统与终端（macOS / Windows Terminal / WSL2）
- [ ] **完整报错原文**（可打码 token 中间段）
- [ ] 身份路径：账号登录 / 官方 Key / 第三方 provider（不要贴 Key）
- [ ] 是否设置了 `HTTP(S)_PROXY`（只说有/无与协议类型，不必暴露内网拓扑）

## 三条原则

1. 先抄报错，再猜原因。
2. 一次只改一个条件。
3. 安装与更新只从已核验来源下载。
