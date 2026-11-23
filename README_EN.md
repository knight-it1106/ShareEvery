<div align="center">

# ShareEvery

**High-Speed Android ↔ Windows USB / Hotspot Network Bridge**

[![Platform](https://img.shields.io/badge/Platform-Android%208%2B%20%7C%20Windows%2010%2F11-007AFF?style=flat-square)](#download--quick-start)
[![Version](https://img.shields.io/badge/Version-v3.7.0-28C759?style=flat-square)](#download--quick-start)
[![Privacy](https://img.shields.io/badge/Privacy-Zero%20Telemetry-5856D6?style=flat-square)](./PRIVACY.md)

[简体中文](./README.md) · [English](./README_EN.md) · [Changelog](./CHANGELOG.md) · [Contributing & Copyright](./CONTRIBUTING.md) · [Privacy](./PRIVACY.md)

</div>

---

## Key Features

- **Native-Speed Throughput**: Prioritizes **USB Tethering (RNDIS)** kernel virtual Ethernet (`<1ms` hop), unlocks OS TCP Auto-Tuning, uses a 64KB zero-GC buffer pool and in-memory DNS caching on Android.
- **Rock-Solid Concurrency & Streaming**: Elastic 1024-thread proxy engine with full bidirectional TCP Half-Close and fast circuit-breaking — built for AI streaming, HTTP/2, gRPC, and IDEs without `unexpected EOF`.
- **Dual Modes**:
  - **HTTP System Proxy (No UAC)**: Auto-configures Windows system proxy with LAN bypass rules (`localhost`, `192.168.*`, `10.*`).
  - **TUN Global Mode (Pro)**: Wintun virtual adapter + built-in DNS-over-TCP forwarder for CLI tools, terminals, and full-system routing.
- **High Availability**: 6-second link heartbeat with seamless failover (RNDIS → Wi-Fi → ADB), crash-safe proxy/route restoration, and one-click **Reset Network**.
- **Unified Modern Design**: Consistent Light/Dark/Auto theme and English/Chinese i18n across Android and Windows.

---

## Trial & Pro Licensing

- **Day 1 (24 Hours)**: Full Pro experience unlocked (TUN Global + Auto Failover + RNDIS).
- **Days 2–8 (7 Days)**: Free Basic trial (HTTP System Proxy mode).
- **Pro License**: Activate once on Android; Windows automatically unlocks offline via **ECDSA P-256** signed JWT verification upon connecting — no internet required on PC.

---

## Download & Quick Start

| Platform | Direct (GitHub Official) | Fast Mirror 1 (CN) | Fast Mirror 2 (CN) |
|---|---|---|---|
| **Windows** (`v3.7.0`, Portable) | [Download .exe](https://github.com/knight-it1106/ShareEvery/releases/download/v3.7.0/ShareEvery-Windows-v3.7.0.exe) | [Mirror 1 .exe](https://gh-proxy.com/https://github.com/knight-it1106/ShareEvery/releases/download/v3.7.0/ShareEvery-Windows-v3.7.0.exe) | [Mirror 2 .exe](https://ghfast.top/https://github.com/knight-it1106/ShareEvery/releases/download/v3.7.0/ShareEvery-Windows-v3.7.0.exe) |
| **Android** (`v3.7.0`, Android 8+) | [Download .apk](https://github.com/knight-it1106/ShareEvery/releases/download/v3.7.0/ShareEvery-Android-v3.7.0.apk) | [Mirror 1 .apk](https://gh-proxy.com/https://github.com/knight-it1106/ShareEvery/releases/download/v3.7.0/ShareEvery-Android-v3.7.0.apk) | [Mirror 2 .apk](https://ghfast.top/https://github.com/knight-it1106/ShareEvery/releases/download/v3.7.0/ShareEvery-Android-v3.7.0.apk) |

1. Install `ShareEvery-Android-v3.7.0.apk` on your phone and tap the power button.
2. Run `ShareEvery-Windows-v3.7.0.exe` on Windows (portable, no installer required).
3. For maximum speed, connect via USB cable and enable **USB Tethering** on Android.

> **Note**: Only the latest official release binaries are hosted under Releases; full version history is available in [CHANGELOG.md](./CHANGELOG.md).  
> **Copyright**: © 2026 ShareEvery (`knight-it1106`). All Rights Reserved. See [LICENSE](./LICENSE) and [CONTRIBUTING.md](./CONTRIBUTING.md) for authorized derivative works.
