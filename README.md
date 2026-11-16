<div align="center">

<img src=".github/nusanx-logo.png" width="136" alt="NusaNx Logo" />

# NusaNx

**On-device Nintendo Switch (`.nsp` / `.xci`) to native iOS / iPadOS ARM64 & Apple Metal Studio**

[![Status](https://img.shields.io/badge/Status-Closed%20Beta-FF3B5C?style=flat-square)](#beta-releases)
[![Platform](https://img.shields.io/badge/Platform-iOS%20%2F%20iPadOS%2026%2B-00C2FF?style=flat-square&logo=apple)](#requirements)
[![Target](https://img.shields.io/badge/Target-Apple%20Silicon%20ARM64-8B5CF6?style=flat-square)](#highlights)
[![Graphics](https://img.shields.io/badge/Graphics-Apple%20Metal%20%28Route%20B%29-10E89B?style=flat-square)](#highlights)
[![Discord](https://img.shields.io/badge/Discord-Join%20Community-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/gme54SrAZn)

</div>

---

## Overview

**NusaNx** transforms legal Nintendo Switch game containers into standalone native iOS / iPadOS `.ipa` applications directly on-device — no companion Mac or external JIT server required during conversion.

Game binaries run natively on Apple Silicon ARM64 while Switch graphics shaders are translated directly into **Apple Metal** on-device.

---

## Highlights

- **On-Device Packaging Pipeline:** Decrypts `.nsp` / `.xci` containers locally with your own `prod.keys`, rewrites ARM64 modules, indexes `RomFS.img`, and packages an installable `.ipa`.
- **On-Device Route B Metal Shaders:** Translates Switch NVN and OpenGL shaders into Metal Shading Language directly on iPad without dynamic shader JIT.
- **Game Artwork & Metadata:** Automatically extracts title metadata and game cover icons from game containers and embeds full iOS/iPadOS `AppIcon` assets into generated `.ipa` files.
- **Multi-Style Studio UI:** Switch live between *Switch Neon*, *Cyber OLED*, *Midnight Pro*, and *Solar Forge* themes, with an adaptive two-column iPad cockpit, built-in SHA-256 IPA verification, and a filterable telemetry console.

---

## Beta Releases

> **NusaNx is currently in active Beta.**  
> Official `.ipa` builds and changelogs will be published on the **Releases** page once public beta builds open. No pre-built releases are available yet.

---

## Community

Join the official Discord server for beta updates, game compatibility notes, and testing discussion:

- **Discord:** [https://discord.gg/gme54SrAZn](https://discord.gg/gme54SrAZn)

---

## Requirements

- **iPad:** Apple M1 chip or newer (`iPadOS 26.0+`)
- **iPhone:** Apple A17 Pro chip or newer (`iOS 26.0+`)
- **Sideloading:** LiveContainer, SideStore, or AltStore *(enable **Increased Memory Limit** for larger titles)*
- **User Files:** Your own legal `prod.keys` and `.nsp` / `.xci` backups

---

## Legal Notice

NusaNx is an independent software project and is not affiliated with Nintendo Co., Ltd. or Apple Inc. This repository contains **zero** decryption keys, firmware files, or copyrighted game assets.

---

## References

Technical inspiration & open-source references: **Ryujinx**, **SPIRV-Cross**, **Atmosphère**, **LibHac**, and **nxnative**.
