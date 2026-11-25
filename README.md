<div align="center">

# ShareEvery

**Android ↔ Windows 极速无线 / 同 Wi-Fi / USB 网络桥接与多设备共享工具**

[![Platform](https://img.shields.io/badge/Platform-Android%208%2B%20%7C%20Windows%2010%2F11-007AFF?style=flat-square)](#下载与安装)
[![Version](https://img.shields.io/badge/Version-v4.0.1-28C759?style=flat-square)](#下载与安装)
[![Privacy](https://img.shields.io/badge/Privacy-Zero%20Telemetry-5856D6?style=flat-square)](./PRIVACY.md)

[简体中文](./README.md) · [English](./README_EN.md) · [更新日志](./CHANGELOG.md) · [二创与版权规范](./CONTRIBUTING.md) · [隐私声明](./PRIVACY.md)

</div>

---

## 为什么选择 ShareEvery？

手机上的高速网络或企业内网隧道，往往难以稳定、满速地共享给电脑端使用——普通热点容易限速、断流、DNS 污染或 IP 漂移。**ShareEvery** 通过双端协同，将手机变成一台零额外开销的桌面级高速网络网关：

- **优先支持同 Wi-Fi 纯无线共享（v4.0 重大升级）**：内置双端局域网动态发现与自定义端口自动同步，手机与电脑连在**同一个 Wi-Fi 下无需开启手机热点**即可直接开启 TUN 全局高速上网，完美适配无法同时开 Wi-Fi 与热点的老旧机型。
- **全场景无线 / 有线自由切换**：支持同 Wi-Fi 无线、USB 网络共享（RNDIS 延迟 `<1ms`）、手机 5GHz 个人热点三种连接姿势；电脑端围绕启动按钮配备圆形连接进度环与实时分步提示。
- **高并发不卡顿、长连接不断流**：独立弹性高并发协程池（最高 1024 并发），完整实现标准双向 TCP 半关闭（Half-Close）与失败节点快速熔断，流畅承载 IDE、AI 流式输出、HTTP/2、gRPC 与大文件下载。
- **双模式独立并行**：
  - **HTTP 系统代理模式（免 UAC）**：自动托管 Windows 系统代理并注入局域网智能绕过规则（`localhost` / `192.168.*` / `10.*` 直连），毫秒级生效。
  - **TUN 全局接管模式（Pro）**：Wintun 虚拟网卡 + 内置防污染 DNS-over-TCP 转发器，接管全系统、命令行（CLI）、开发工具与游戏流量。
- **安全可控防蹭网**：支持「自动放行 / 手动审批」接入放权双模式（含后台高优先级通知审批）与移动设备免装共享（支持 iPhone / iPad / Android）。

### 三种连接方式优缺点对比（按需选择）

| 连接方式 | 推荐场景 | 优点 | 缺点 / 注意事项 |
|---|---|---|---|
| **📶 同 Wi-Fi 无线直连（优先推荐）** | 家庭 / 宿舍 / 普通办公室内 | **无需开热点、不挑旧手机硬件**、省电不发烫、纯无线自动发现并同步自定义端口、支持电脑 TUN 全局 | 若公共 Wi-Fi（酒店/校园网）开启了「AP 设备隔离」导致同网不可互访，需切换下方方式 |
| **🔌 USB 一线直连（最稳满速）** | 长时间重度办公 / 游戏 / 公共 Wi-Fi 受限 | **延迟 `<1ms` 零抖动、边用边充电**、100% 穿透一切 Wi-Fi 设备隔离、最高物理级安全隔离 | 需要插一根 USB 数据线 |
| **📡 手机个人热点（户外无线）** | 户外 / 出差无 Wi-Fi 环境 | 无需路由器即可无线连接并支持电脑 TUN 全局（开启 5GHz 频段可达 150~400 Mbps） | 长时间高负载转发略耗电发热，且部分旧手机硬件不支持 Wi-Fi 与热点同时开启 |

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

### 一键高速下载（最新版 `v4.0.1`）

> 中国大陆用户未配置代理时，推荐直接点击下方 **国内高速镜像线路** 一键下载；下载完成后可核对 [SHA256SUMS.txt](https://gh-proxy.com/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.1/SHA256SUMS.txt) 确保安装包 100% 为官方原版。

| 平台 | 国内高速线路 1（推荐） | 国内高速线路 2（备用） | GitHub 官方源 |
|---|---|---|---|
| **Windows 电脑端** (`v4.0.1`, 绿色免安装) | [⚡ 极速下载 .exe](https://gh-proxy.com/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.1/ShareEvery-Windows-v4.0.1.exe) | [备用线路 .exe](https://ghfast.top/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.1/ShareEvery-Windows-v4.0.1.exe) | [官方直链 .exe](https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.1/ShareEvery-Windows-v4.0.1.exe) |
| **Android 手机端** (`v4.0.1`, Android 8+) | [⚡ 极速下载 .apk](https://gh-proxy.com/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.1/ShareEvery-Android-v4.0.1.apk) | [备用线路 .apk](https://ghfast.top/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.1/ShareEvery-Android-v4.0.1.apk) | [官方直链 .apk](https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.1/ShareEvery-Android-v4.0.1.apk) |

### 快速上手

1. **Android 端**：安装 `ShareEvery-Android-v4.0.1.apk`，打开后点击主电源开关开启共享（建议按提示关闭电池优化）。
2. **Windows 端**：直接运行单文件版 `ShareEvery-Windows-v4.0.1.exe`（免安装、绿色便携）。
3. **无线优先（同 Wi-Fi 免热点）**：手机与电脑连在**同一个 Wi-Fi** 下，直接点击电脑端启动按钮即可自动发现手机、同步自定义端口并开启 HTTP 或 TUN 全局共享；如需极致低延迟或穿透公共 Wi-Fi 隔离，插上 USB 线开启「USB 网络共享」即可。
4. **共享给另一部手机 / iPad（免装客户端）**：在 Android 端开启「手机 / 平板免装共享」，另一部手机或 iPad 连入同 Wi-Fi 或热点并按顶部「指南」填入代理/PAC 即可上网（免费每日 90 分钟 / 单次 45 分钟，Pro 无限时长）。

> **说明**：为保障安全，[Releases](../../releases) 页面**仅保留最新正式版安装包**；所有历史版本的更新记录均可在 [CHANGELOG.md](./CHANGELOG.md) 中公开查阅。

---

## 隐私、版权与二次创作

- **隐私承诺**：ShareEvery 是纯粹的**本地直连工具**，所有网络流量仅在您的电脑与手机之间通过 USB 或局域网传输，**绝不经过任何第三方中转服务器，不收集任何日志或隐私数据**。详见 [PRIVACY.md](./PRIVACY.md)。
- **版权声明**：本项目采用 [All Rights Reserved](./LICENSE) 专有版权保护（Copyright © 2026 ShareEvery / `knight-it1106`）。如需二次创作或功能共创，请先阅读 [二创与版权规范](./CONTRIBUTING.md) 申请在主项目下创建分支开发并保留原作者署名。
