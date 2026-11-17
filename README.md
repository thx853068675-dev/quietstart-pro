# 轻启 Pro

面向 HarmonyOS 的自动化与网络工具。

本仓库用于发布预览版 HAP、更新说明与问题反馈，目前不提供完整应用源码。

## 下载

**[下载 1.0.1 预览版 HAP](https://github.com/thx853068675-dev/quietstart-pro/releases/download/v1.0.1-preview-130125/quietstart-pro-1.0.1-preview-130125-unsigned.hap)** · [发布说明](https://github.com/thx853068675-dev/quietstart-pro/releases/tag/v1.0.1-preview-130125) · [校验文件](https://github.com/thx853068675-dev/quietstart-pro/releases/download/v1.0.1-preview-130125/SHA256SUMS.txt)

| 项目 | 信息 |
| --- | --- |
| 应用版本 | 1.0.1 预览版 |
| 构建版本 | 130125 |
| 包名 | `com.tonghongxiang.quietstart.pro` |
| 制品格式 | HAP，单 `entry` 主模块 |
| 签名 | 无签名，安装前需要自行签名 |
| 文件大小 | 28,281,682 字节 |

下载无签名 HAP 后，使用自己的开发者身份签名安装。无需解压。

Pro 使用独立包名，可与普通轻启同时安装；两者不会自动共享应用数据。

## 功能

- 自动化：页面识别、学习与手动规则、工具包运行。
- 网络：订阅与分流配置、VPN 接管、本机 HTTP／SOCKS5 代理、MITM 与规则处理。
- 共享：无线调试连接、应用列表、图标缓存与全局设置。

概览页的网络开关控制整个网络进程。网络页左上角的圆形开关控制 VPN，本机代理使用自己的开关。概览网络关闭时，本机代理开关禁用，已保存配置保留。

## 预览说明

本版已通过本地回归与 SDK release 构建检查。1.0.1 在 nova 14 上实测了规则模式分流（国内直连、国外经节点、广告阻断）、覆盖安装后的 VPN 恢复、后台内存与网络页 CPU；Pura X 尚未验证。VPN 模式切换时已有连接可能短暂重连。

已知问题：自定义分流订阅目前仍沿用系统 DNS，遇到被污染的域名可能打不开；内置 MyClash 规则走分流 DNS，不受影响。MITM 需按实际需求配置规则与用户证书。

问题反馈请提交 [Issue](https://github.com/thx853068675-dev/quietstart-pro/issues)，附设备型号、系统版本、构建版本和复现步骤。

## 校验

```text
700a0a8e3aac05a70dad11868dbc5d47eb980e12277ed4b982601bb23361802f  quietstart-pro-1.0.1-preview-130125-unsigned.hap
```

更新记录见 [CHANGELOG.md](CHANGELOG.md)。
