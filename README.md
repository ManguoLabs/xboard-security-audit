# XBoard 订阅安全审计与账号关联分析

用于理解 XBoard 内鬼查询、XBoard 查内鬼、订阅共享、Token 多 IP、账号关联和安全审计的证据模型与排查方法。

> 多 IP 不等于“100% 内鬼”。家庭 NAT、移动网络、旅行、设备切换和公司网络都可能产生合理的 IP 变化。风险评分只能辅助调查，不能作为唯一封号依据。

## 可以分析什么

- 一个 Token 在多个 IP 或地区出现
- 同一出口 IP 关联多个账号
- 订阅 IP、登录 IP 与真实连接 IP 的差异
- 订阅链接泄露、转发或异常使用线索
- Soga 真实连接 IP 与连接记录

## 审计原则

先定义时间窗口和正常行为基线，再关联 Token、账号、IP、设备与连接事件。对高风险结果进行人工复核，并保留可解释的证据链。

## 文档

- [Token 多 IP 如何分析](docs/token-multi-ip.md)
- [账号共享的证据与误判](docs/account-sharing.md)
- [IP 与账号关联方法](docs/ip-correlation.md)
- [Soga 真实连接 IP](docs/soga-real-ip.md)
- [常见问题 FAQ](FAQ.md)

## Manguo Labs

产品说明：[XBoard 订阅安全审计](https://manguolabs.com/xboard-security-audit/)

需要评估现有数据源时，可通过 [@ManguoShop_bot](https://t.me/ManguoShop_bot) 咨询。请勿在公开 Issue 中粘贴 Token、用户数据、IP 明细或内部日志。
