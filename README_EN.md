<div align="center">

# ShareEvery

**High-Speed Android ↔ Windows USB / Hotspot Network Bridge**

[![Platform](https://img.shields.io/badge/Platform-Android%208%2B%20%7C%20Windows%2010%2F11-007AFF?style=flat-square)](#download--quick-start)
[![Version](https://img.shields.io/badge/Version-v4.0.2-28C759?style=flat-square)](#download--quick-start)
[![Privacy](https://img.shields.io/badge/Privacy-Zero%20Telemetry-5856D6?style=flat-square)](./PRIVACY.md)

[简体中文](./README.md) · [English](./README_EN.md) · [Changelog](./CHANGELOG.md) · [Contributing & Copyright](./CONTRIBUTING.md) · [Privacy](./PRIVACY.md)

</div>

---

## Key Features (v4.0 Major Release)

- **Wireless-First Same-Wi-Fi Sharing (No Hotspot Required)**: Built-in LAN UDP dynamic discovery automatically detects your phone on the **same Wi-Fi** and syncs custom HTTP/SOCKS5 ports — even on older phones that cannot run Wi-Fi + Hotspot simultaneously, with full PC TUN Global support.
- **Connection Modes & Trade-offs**:
  - **Same Wi-Fi Wireless (Recommended Indoors)**: No hotspot needed, cool & battery-friendly, instant auto-discovery; may be blocked on public Wi-Fi with AP isolation.
  - **USB Tethering / RNDIS (Most Stable)**: `<1ms` latency, charges while sharing, bypasses all public Wi-Fi AP isolation; requires a USB cable.
  - **Phone Hotspot (Best Outdoors)**: Full wireless TUN Global on the go (150–400 Mbps on 5GHz); uses more battery under heavy load.
- **Circular Progress Ring & Zero-Friction Connect**: Smooth circular progress ring around the PC launch button with live step status, handshake-first anti-false-positive flow, and dual-mode access control (`Auto Allow` / `Manual Approval` with background notifications).

---

## Trial & Pro Licensing

- **Day 1 (24 Hours)**: Full Pro experience unlocked (TUN Global + Auto Failover + RNDIS).
- **Days 2–8 (7 Days)**: Free Basic trial (HTTP System Proxy mode).
- **Pro License**: Activate once on Android; Windows automatically unlocks offline via **ECDSA P-256** signed JWT verification upon connecting — no internet required on PC.

---

## Download & Quick Start

| Platform | Direct (GitHub Official) | Fast Mirror 1 (CN) | Fast Mirror 2 (CN) |
|---|---|---|---|
| **Windows** (`v4.0.2`, Portable) | [Download .exe](https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.2/ShareEvery-Windows-v4.0.2.exe) | [Mirror 1 .exe](https://gh-proxy.com/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.2/ShareEvery-Windows-v4.0.2.exe) | [Mirror 2 .exe](https://ghfast.top/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.2/ShareEvery-Windows-v4.0.2.exe) |
| **Android** (`v4.0.2`, Android 8+) | [Download .apk](https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.2/ShareEvery-Android-v4.0.2.apk) | [Mirror 1 .apk](https://gh-proxy.com/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.2/ShareEvery-Android-v4.0.2.apk) | [Mirror 2 .apk](https://ghfast.top/https://github.com/knight-it1106/ShareEvery/releases/download/v4.0.2/ShareEvery-Android-v4.0.2.apk) |

1. Install `ShareEvery-Android-v4.0.2.apk` on your phone and tap the power button.
2. Run `ShareEvery-Windows-v4.0.2.exe` on Windows (portable, no installer required).
3. **Wireless First**: Connect phone and PC to the **same Wi-Fi** (no hotspot needed) and click Start on PC — or plug in USB Tethering for `<1ms` latency.
4. **Share to Another Phone / iPad (Clientless)**: Enable **Share to Other Mobile Devices** on Android and follow the built-in Guide to set the PAC URL on iOS/iPadOS/Android (Free: 90 min/day, 45 min/session; Pro: unlimited).

> **Note**: Only the latest official release binaries are hosted under Releases; full version history is available in [CHANGELOG.md](./CHANGELOG.md).  
> **Copyright**: © 2026 ShareEvery (`knight-it1106`). All Rights Reserved. See [LICENSE](./LICENSE) and [CONTRIBUTING.md](./CONTRIBUTING.md) for authorized derivative works.
