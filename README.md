# 轻启 Pro

面向 HarmonyOS 的自动化与网络工具。

本仓库用于发布预览版 HAP、更新说明与问题反馈，目前不提供完整应用源码。

## 下载

**[下载 1.0.6 预览版 HAP](https://github.com/thx853068675-dev/quietstart-pro/releases/download/v1.0.6-preview-130437/quietstart-pro-1.0.6-preview-130437-unsigned.hap)** · [发布说明](https://github.com/thx853068675-dev/quietstart-pro/releases/tag/v1.0.6-preview-130437) · [校验文件](https://github.com/thx853068675-dev/quietstart-pro/releases/download/v1.0.6-preview-130437/SHA256SUMS.txt)

| 项目 | 信息 |
| --- | --- |
| 应用版本 | 1.0.6 预览版 |
| 构建版本 | 130437 |
| 包名 | `com.tonghongxiang.quietstart.pro` |
| 制品格式 | HAP，单 `entry` 主模块 |
| 签名 | 无签名，安装前需要自行签名 |
| 文件大小 | 22,172,848 字节 |

下载 HAP 后，使用自己的开发者身份签名安装。覆盖安装时需沿用原签名身份。

Pro 使用独立包名，可与普通轻启同时安装。两者的应用数据各自保存。

## 功能

- 自动化：页面识别、学习与手动规则、工具包运行。
- 网络：订阅与分流配置、VPN 接管、本机 HTTP／SOCKS5 代理、MITM 与规则处理。
- 共享：无线调试连接、应用列表、图标缓存与全局设置。

概览页的网络开关控制整个网络进程。网络页左上角的圆形开关控制 VPN，本机代理使用自己的开关。概览网络关闭时，本机代理开关禁用，已保存配置保留。

## 订阅兼容性

从旧版升级后，请刷新一次受影响的在线订阅，或重新导入原本地文件，以读取服务商指定的节点 DNS。

## 预览版验证

Pura 70 已验证原链接导入、AnyTLS 节点测速及系统浏览器经 VPN 访问 HTTPS 站点。实测全局代理与直连模式的浏览器出口不同。32 项相关回归通过。

MITM 需按实际需求配置规则与用户证书。

问题反馈请提交 [Issue](https://github.com/thx853068675-dev/quietstart-pro/issues)，附设备型号、系统版本、构建版本和复现步骤。

## 校验

```text
c658130dd9a21896511fa5ca1fa37d75f159d94fe735cd0cb639c6a3144e7454  quietstart-pro-1.0.6-preview-130437-unsigned.hap
```

更新记录见 [CHANGELOG.md](CHANGELOG.md)。
