# QMS Audio OS · 官方发行下载中心

**七木发烧数播操作系统（QMS Audio OS）** 是一款专为纯音乐聆听打造的 x86_64 专用声学操作系统（非通用桌面系统修改版）。底层采用纯 C 语言 Zero-Copy 推流引擎与 Bit-Perfect 硬件直通架构，全面释放 Hi-Fi 解码器潜能。

> **免责与仓库说明**：本公开仓库仅用于托管 QMS Audio OS 官方正式发布的 **安装镜像（`.iso`）**、**系统升级包（`.qpkg`）** 与 **SHA-256 校验文件**。前往下载页面 👉 [**GitHub Releases**](https://github.com/cqtvro/qms-download/releases/latest)

---

## 核心技术特性

- **Bit-Perfect 源码直出**：纯 C 推流直通 ALSA 硬件层，原生支持 `Native DSD64 ~ DSD512` / `DoP DSD` 与最高 `PCM 768kHz`（XMOS）/ `384kHz`（Amanero Combo384），内置 1-bit Sigma-Delta 硬件兼容性降采样。
- **SACD ISO / CUE 原盘直解**：内存扇区级直读 `SACD ISO` 与 `CUE` 整轨虚拟分轨，支持 `FLAC`、`WAV`、`APE`、`DSF`、`DFF`、`AIFF`、`ALAC/M4A`、`MP3`，并原生融合中文 XML 元数据与专辑封面。
- **6 档经典名胆调音 & 10 段录音室 EQ**：支持 `Bypass` 直通与 `300B`、`KT88`、`ECC83`、`2A3`、`EL34` 偶次谐波毫秒热切换；配备 64-bit 浮点 IIR `10 段 EQ`（`31.25Hz ~ 16kHz`，`-12.0dB ~ +12.0dB`）与智能防削波余量控制。
- **双端视觉控台与 4 款美学主题**：提供黑曜石、黑胡桃、暖橡木、银拉丝四套界面风格；兼备 PC 专业三栏控台（1024 点实时 FFT 频谱）与手机触控端（麦景图双通道 RMS 电平表与黑胶交互）。
- **全场景音源融合与双向投流**：支持本地盘/移动硬盘即插即扫、局域网 `SMB` / `NFS` 自动发现挂载与拖拽传歌、5 大云盘（百度 / 阿里云盘 / 夸克 / 115 / WebDAV）直出、网易云无损直通、`AirPlay` / `DLNA` 双向投流，以及「音乐播不停」无感续航。
- **发烧纯净模式 & 安全可靠架构**：支持一键切换至发烧极简纯净模式（关闭常驻网盘与流媒体服务释放 `200MB+` 内存）、USB DAC 热插拔自动识别、硬件防爆音开机静音守护，以及纯净单系统直装、GitHub 一键在线 OTA 升级与 A/B 双槽位保护。

---

## 版本矩阵（x86_64 架构）

| 版本定位 | 内核特性 | 商业授权定价 |
| :--- | :--- | :--- |
| **QMS Pro 商业专业版** | Linux LTS 标准内核，全功能发烧声学底座 | **¥299 / 永久买断** |
| **QMS-RT 纯血实时至尊版** | `Linux PREEMPT_RT` 微秒级实时声学内核 | **¥599 / 永久买断**（Pro 老用户享 3 天试听及补差价 ¥300 升级） |

---

## 最新版本直链下载（ISO：`v7.2.7 Pure` / 固件升级包：`v7.2.8`）

> 国际化纯净发行版仅包含纯正 QMS 自主系统，安装完成后即自带 **GitHub 官方源一键在线 OTA 升级** 能力：装完 `v7.2.7 Pure` 镜像开机后，即可直接在 Web 控制台 **系统设置 → 固件升级** 一键热升级至最新 `v7.2.8`（修复安卓网易云 DLNA 投流兼容）。

### 1. 全新装机 ISO 镜像（Pure Single-OS）

| 版本 | 内核 | 大小 | 下载地址 | SHA-256 校验 |
| :--- | :--- | :--- | :--- | :--- |
| **QMS-RT 纯血实时版** | `6.6.142-qms-rt` (`PREEMPT_RT`) | 531 MiB | [QMS-Audio-RT-v7.2.7-Pure-x86_64.iso](https://github.com/cqtvro/qms-download/releases/download/v7.2.7/QMS-Audio-RT-v7.2.7-Pure-x86_64.iso) ([.sha256](https://github.com/cqtvro/qms-download/releases/download/v7.2.7/QMS-Audio-RT-v7.2.7-Pure-x86_64.iso.sha256)) | `f620bddd527b31b93a7bd68a0ba09af7240afc61aaacafe3278a35fd5db4b163` |
| **QMS Pro 商业标准版** | `6.6.142-0-lts` (`LTS`) | 597 MiB | [QMS-Audio-PRO-v7.2.7-Pure-x86_64.iso](https://github.com/cqtvro/qms-download/releases/download/v7.2.7/QMS-Audio-PRO-v7.2.7-Pure-x86_64.iso) ([.sha256](https://github.com/cqtvro/qms-download/releases/download/v7.2.7/QMS-Audio-PRO-v7.2.7-Pure-x86_64.iso.sha256)) | `b4b636b61709082c235ba3f22b4a29405cd7e1952204a0ff18b90907095545e2` |

### 2. 已有设备升级包（`v7.2.8` `.qpkg`）

| 版本 / 适用范围 | 大小 | 下载地址 | SHA-256 校验 |
| :--- | :--- | :--- | :--- |
| **RT 轻量 OTA 包**（`v7.1.0+`） | 9.08 MB | [QMS-Upgrade-v7.2.8-Lite-RT.qpkg](https://github.com/cqtvro/qms-download/releases/download/v7.2.8/QMS-Upgrade-v7.2.8-Lite-RT.qpkg) | `4ce5254bbaa6a0926a553609cea60d98547f8082e00ba002ccb9e6da732f1007` |
| **PRO 轻量 OTA 包**（`v7.1.0+`） | 6.38 MB | [QMS-Upgrade-v7.2.8-Lite-PRO.qpkg](https://github.com/cqtvro/qms-download/releases/download/v7.2.8/QMS-Upgrade-v7.2.8-Lite-PRO.qpkg) | `e2f9dbed46de296b01f817d94e549cfc9a30ea48a09b98241b01f939fbe3e782` |
| **RT 全量跨代包**（全版本通用） | 263.54 MB | [QMS-Upgrade-v7.2.8-RT.qpkg](https://github.com/cqtvro/qms-download/releases/download/v7.2.8/QMS-Upgrade-v7.2.8-RT.qpkg) | `1718cfc1b939aec0ba90100eb3f2e08e8fc4aafc5a2b45d845448f5b64b3f11b` |
| **PRO 全量跨代包**（全版本通用） | 263.54 MB | [QMS-Upgrade-v7.2.8-PRO.qpkg](https://github.com/cqtvro/qms-download/releases/download/v7.2.8/QMS-Upgrade-v7.2.8-PRO.qpkg) | `84929ee92a968dc360022bfda1fe0be81ba807024da03ce7b08c87f6273db282` |

---

## 安装与升级指南

### 1. 全新装机（`.iso` 镜像）
1. 在上方表格或 [Releases](https://github.com/cqtvro/qms-download/releases/latest) 下载对应版本的 `.iso` 镜像文件。
2. 使用 **Rufus**（建议选择 **DD 镜像模式**）或 **balenaEtcher** 将 `.iso` 写入 U 盘。
3. 在主板 BIOS 中关闭 **Secure Boot（安全启动）**，设置为 UEFI USB 启动；进入系统后使用同局域网浏览器打开屏幕显示的 IP，即可在 Web 控制台点击 **一键安装至机内硬盘**（安装完毕拔掉 U 盘重启，即可直接使用 GitHub 一键在线 OTA）。

### 2. 系统平滑升级（`.qpkg` 升级包）
- 已有 `v7.2.7` / `v7.2.6+` 设备可在 Web 控制台 **系统设置 → 固件升级** 直接点击 **一键在线 OTA 升级**，系统会自动选择适配的轻量包或全量包并校验 SHA-256。
- 也可手动下载对应版本的 `.qpkg` 升级包上传升级（无需重装系统或重新配置曲库与授权，支持 A/B 安全双槽位保护）。

### 3. 文件完整性校验（`.sha256`）
下载大文件后，建议核对与同目录 `.sha256` 文件是否一致：

```powershell
# Windows PowerShell 校验示例
Get-FileHash .\<下载的文件名> -Algorithm SHA256
```

```bash
# Linux / macOS 校验示例
sha256sum -c <文件名>.sha256
```

---

## 官方入口

- 🌐 **官方网站**：[https://www.284868.xyz](https://www.284868.xyz)
- 🔐 **自助兑换 / 授权与升级中心**：[https://wx.284868.xyz/qms-auth/](https://wx.284868.xyz/qms-auth/)
- 📦 **官方安装包下载列表**：[https://github.com/cqtvro/qms-download/releases](https://github.com/cqtvro/qms-download/releases)

---

Copyright © 2026 七木发烧数播团队 (QMS Audio OS). All rights reserved.
