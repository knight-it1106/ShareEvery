<div align="center">

# ShareEvery

**Android ↔ Windows 极速 USB / 热点网络桥接与多设备共享工具**

[![Platform](https://img.shields.io/badge/Platform-Android%208%2B%20%7C%20Windows%2010%2F11-007AFF?style=flat-square)](#下载与安装)
[![Version](https://img.shields.io/badge/Version-v3.4.1-28C759?style=flat-square)](#下载与安装)
[![Privacy](https://img.shields.io/badge/Privacy-Zero%20Telemetry-5856D6?style=flat-square)](./PRIVACY.md)

[简体中文](./README.md) · [English](./README_EN.md) · [隐私与安全声明](./PRIVACY.md)

</div>

---

## 为什么选择 ShareEvery？

手机上的高速网络或企业内网隧道，往往难以稳定、满速地共享给电脑端使用——普通热点容易限速、断流、DNS 污染或 IP 漂移。**ShareEvery** 通过双端协同，将手机变成一台零额外开销的桌面级高速网络网关：

- **逼近手机原生满速**：自动优先识别 **USB 网络共享（RNDIS 虚拟以太网）**，释放内核 TCP Auto-Tuning 窗口自动调优 + 64KB 零 GC 缓冲池 + 手机端内存 DNS 缓存，实测延迟 `<1ms`，吞吐比肩手机本地。
- **高并发不卡顿、长连接不断流**：独立弹性高并发协程池（最高 1024 并发），完整实现标准双向 TCP 半关闭（Half-Close）与失败节点快速熔断，流畅承载 IDE、AI 流式输出、HTTP/2、gRPC 与大文件下载。
- **双模式一键切换**：
  - **HTTP 系统代理模式（免 UAC）**：自动托管 Windows 系统代理并注入局域网智能绕过规则（`localhost` / `192.168.*` / `10.*` 直连），毫秒级生效。
  - **TUN 全局接管模式（Pro）**：Wintun 虚拟网卡 + 内置防污染 DNS-over-TCP 转发器，接管全系统、命令行（CLI）、开发工具与游戏流量。
- **高可用防断网兜底**：6 秒链路心跳检测，USB 松动自动无感热切至 ADB / Wi-Fi 备用通道；进程退出或异常崩溃自动还原系统代理与路由，内置 **一键重置网络**。
- **双端统一极简美学**：Android 与 Windows 共用同一套设计语言（浅色 / 深色 / 跟随系统 + 中英双语切换），全屏沉浸无广告。

---

## 免费体验与 Pro 授权说明

为让您充分体验 ShareEvery 的极致网速与稳定性，我们提供阶梯式免费试用：

| 阶段 | 权益范围 | 说明 |
|---|---|---|
| **首日全量体验（24 小时）** | **全部 Pro 功能免费开放** | 完整体验 RNDIS 极速直连、TUN 全局接管、断线无感热切 |
| **基础版试用（随后 7 天）** | HTTP 系统代理模式 + 手动连接 | 持续验证日常办公与浏览体验 |
| **Pro 永久买断版** | **永久解锁全部功能** | 含 TUN 全局、断线无感热切、多设备管理与 v3.x 免费更新 |

> 采用 **手机端在线鉴权 + 电脑端 ECDSA P-256 本地离线验签** 架构：只需在手机端激活一次，电脑通过 USB / Wi-Fi 连接手机后即自动离线解锁 Pro，电脑全程无需联网。

---

## 下载与安装

请前往右侧 **[Releases](../../releases)** 页面下载最新版本安装包：

1. **Android 端**：安装 `ShareEvery-Android-v3.4.1.apk`，打开后点击主电源开关开启共享（建议按提示关闭电池优化）。
2. **Windows 端**：直接运行单文件版 `ShareEvery-Windows-v3.4.1.exe`（免安装、绿色便携）。
3. **满速推荐姿势**：用 USB 数据线连接电脑，在手机开启 **「USB 网络共享」**，电脑端会自动识别 RNDIS 极速通道，一键连接即可起飞。

> 所有 Release 安装包均提供 `SHA256SUMS.txt` 哈希校验值，欢迎自行核验。

---

## 隐私与安全承诺

ShareEvery 是纯粹的**本地直连工具**，所有网络流量仅在您的电脑与手机之间通过 USB 或局域网传输，**绝不经过任何第三方中转服务器，不收集任何日志或隐私数据**。详见 [PRIVACY.md](./PRIVACY.md)。
