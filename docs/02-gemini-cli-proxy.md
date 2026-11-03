# Gemini CLI 代理与 fetch failed

配套：[Gemini CLI 国内代理](https://nano-banana.lol/how-to/gemini-cli-proxy-china)。

## 先抄完整报错

同样是「连不上」，可能是：

- DNS / 防火墙
- 代理协议不匹配（HTTP 代理 vs SOCKS）
- TLS 被中间人设备干扰
- 账号/地区策略提示（文案以客户端原文为准）

**一次只改一个条件。**

## 环境变量思路（示意）

许多 Node CLI 尊重：

```bash
export HTTPS_PROXY=http://127.0.0.1:7890
export HTTP_PROXY=http://127.0.0.1:7890
# 若工具支持 NO_PROXY，把本地服务排除
```

端口与协议以你本机代理客户端为准；不要照抄他人端口。

## 排错顺序

1. 浏览器或 `curl -I` 经同一代理能否访问目标域名。
2. CLI 是否读到了 `HTTPS_PROXY`（新开终端再试）。
3. 公司 SSL 解密证书是否导致校验失败——**不要**用关闭校验当长期方案。
4. 仍失败：记录客户端版本、代理类型、完整报错，再对照站内文或开 Issue（脱敏）。

## 和「地区不支持」提示

若报错明确是资格/地区策略，换代理不一定能合规解决；以官方账号状态与条款为准。

返回：[安装](01-gemini-cli-install.md) · [CC Switch](03-cc-switch.md)
