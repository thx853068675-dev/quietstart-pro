# 轻启 Pro

面向 HarmonyOS 的自动化与网络工具。

本仓库用于发布预览版 HAP、更新说明与问题反馈，目前不提供完整应用源码。

## 下载

**[下载 1.0.0 预览版 HAP](https://github.com/thx853068675-dev/quietstart-pro/releases/download/v1.0.0-preview-130070/quietstart-pro-1.0.0-preview-130070-unsigned.hap)** · [发布说明](https://github.com/thx853068675-dev/quietstart-pro/releases/tag/v1.0.0-preview-130070) · [校验文件](https://github.com/thx853068675-dev/quietstart-pro/releases/download/v1.0.0-preview-130070/SHA256SUMS.txt)

| 项目 | 信息 |
| --- | --- |
| 应用版本 | 1.0.0 预览版 |
| 构建版本 | 130070 |
| 包名 | `com.tonghongxiang.quietstart.pro` |
| 制品格式 | HAP，单 `entry` 主模块 |
| 签名 | 无签名，安装前需要自行签名 |
| 文件大小 | 27,756,178 字节 |

下载无签名 HAP 后，使用自己的开发者身份签名安装。无需解压。

Pro 使用独立包名，可与普通轻启同时安装；两者不会自动共享应用数据。

## 功能

- 自动化：页面识别、学习与手动规则、工具包运行。
- 网络：订阅与分流配置、VPN 接管、本机 HTTP／SOCKS5 代理、MITM 与规则处理。
- 共享：无线调试连接、应用列表、图标缓存与全局设置。

概览页的网络开关控制整个网络进程。网络页左上角的圆形开关控制 VPN，本机代理使用自己的开关。概览网络关闭时，本机代理开关禁用，已保存配置保留。

## 预览说明

本版已通过本地回归与 SDK release 构建检查，130070 尚未完成独立实机验收。VPN 模式切换时已有连接可能短暂重连。部分设备上 VPN 暂停后本机代理可能延后停止，该问题仍在定位。MITM 需按实际需求配置规则与用户证书，导入规则的兼容性以支持范围为准。

问题反馈请提交 [Issue](https://github.com/thx853068675-dev/quietstart-pro/issues)，附设备型号、系统版本、构建版本和复现步骤。

## 校验

```text
b21d4ec0ad027ad3468dacfd78a154ec3b9cbbb6ed2a6dcee86d80e4684fd1a7  quietstart-pro-1.0.0-preview-130070-unsigned.hap
```

更新记录见 [CHANGELOG.md](CHANGELOG.md)。
