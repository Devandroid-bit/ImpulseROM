# Impulse ROM

One UI 8.5 / Android 16 for the **Samsung Galaxy Note10+ Exynos
(`d2s` / `SM-N975F`)**. Impulse ROM is a modified GPLv3 fork of
[EternityROM](https://github.com/Ocin4ever/EternityROM), built on Salvo
Giangreco's UN1CA build system. Original authorship, copyright notices and
upstream credits are preserved.

**Current download: v1.0 Alpha 2 (1 September 2026), a test build.**
Its accompanying release notes report offline validation but no device boot
or runtime testing. All hardware features and a clean installation still
require testing on this ZIP. This port supports SM-N975F only; the inherited
upstream device list below does not extend Impulse's tested support.

- [Download — Google Drive](https://drive.google.com/drive/folders/1BlQ1hBhLhhRsLkH6P1ozAfAJ7xOlbzKK?usp=drive_link)
- [Alpha 2 files](https://drive.google.com/drive/folders/1vFBMG9UuvbmCtLBbB1dLnoBBvsxceyC6)
- [Alpha 2 release notes / known issues](https://drive.google.com/file/d/1sUQ1XYNcOMyJuh9KMnO7xTxLjt6NxAX7/view?usp=drivesdk)
- [Impulse XDA thread](https://xdaforums.com/t/rom-alpha-d2s-sm-n975f-android-16-impulse-rom-v1-0-one-ui-8-5-for-n10.4800645/)
- [Installation](docs/INSTALL.md) · [Build instructions](BUILDING.md)
- [Release source records](docs/source-provenance.md) · [Kernel source details](docs/kernel-source.md) · [Authorship and licences](NOTICE.md)

```text
File: ImpulseROM_v1.0-oneui85-alpha2_@c83e070e-dirty_20260901_d2s-sign.zip
Size: 5,800,045,146 bytes
SHA-256: 14cc19c811d4f0fcb39a429651fc26a17881eab4e233adbc38a9869cccf1504c
```

The checksum is copied from the accompanying checksum file and release notes;
it has not been independently recomputed during this documentation update.
The flashable ZIP itself is unsigned. Verify its SHA-256 before flashing.
Alpha 1 and Alpha 2 were built from uncommitted working trees; the current
public source snapshot is not claimed to reproduce those ZIPs exactly.

## Upstream EternityROM documentation

The following upstream description, device list, features and credits are
retained for attribution and historical context. They are not a verification
of those features or devices on Impulse's Android 16 builds.

<p align="center">
  <a href="https://github.com/Ocin4ever/EternityROM/blob/fifteen/LICENSE"><img loading="lazy" src="https://img.shields.io/github/license/Ocin4ever/EternityROM?style=for-the-badge&logo=github"/></a>
  <a href="https://github.com/Ocin4ever/EternityROM/commits/fifteen"><img loading="lazy" src="https://img.shields.io/github/last-commit/Ocin4ever/EternityROM/fifteen?style=for-the-badge"/></a>
  <a href="https://github.com/Ocin4ever/EternityROM/stargazers"><img loading="lazy" src="https://img.shields.io/github/stars/Ocin4ever/EternityROM?style=for-the-badge"/></a>
  <a href="https://github.com/Ocin4ever/EternityROM/graphs/contributors"><img loading="lazy" src="https://img.shields.io/github/contributors/Ocin4ever/EternityROM?style=for-the-badge"/></a>
</p>
<p align="center">EternityROM is a work-in-progress custom firmware for Samsung Galaxy Note10 series (Exynos).</p>

<p align="center">
  <a href="https://t.me/unicarom">💬 Telegram</a>
  •
  <a href="https://xdaforums.com/t/port-rom-14-eternityrom-v4-0-oneui-6-1-1-for-n10-s10-series.4670331/">🚀 XDA</a>
</p>

# What is EternityROM?
EternityROM is a work-in-progress custom firmware for Samsung Galaxy devices. It's based on the latest and greatest iteration of Samsung's UX and it also includes additional features and tweaks to ensure the best possible experience out of the box.
It is based on the UN1CA build system which allows automatic downloading/extraction of the firmware, applying the required patches and generating a flashable zip/tar package for the specified target device.

Any form of contribution, suggestions, bug report or feature request for the project will be welcome.

# Supported Devices
- Note 10:
  - d1 - N970F
- Note 10 5G:
  - d1xks - N971N
- Note10+:
  - d2s - N975F
- Note10+ 5G:
  - d2x - N976B
  - d2xks - N976N

# Features
- Based on the latest stable OneUI 7 Galaxy S24+ firmware
- All software features from S25 Ultra
- Slightly Debloated
- Partially DeKnoxed
- Full SELinux Support
- Full Galaxy AI support
- Completely upstreamed kernels 4.14
- High end animations
- Native/live blur support
- Adaptive color tone support
- Debloated from useless system services/additional apps
- [BluetoothLibraryPatcher](https://github.com/3arthur6/BluetoothLibraryPatcher) included
- [KnoxPatch](https://github.com/salvogiangri/KnoxPatch) implemented in system frameworks
- Extra mods (Disable Secure Flag, OutDoor mode, more coming soon)
- Extra CSC features (Call recording, Network speed in status bar)

# Licensing
This project is licensed under the terms of the [GNU General Public License v3.0](LICENSE). External dependencies might be distributed under a different license, such as:
- [android-tools](https://github.com/nmeum/android-tools), licensed under the [Apache License 2.0](https://github.com/nmeum/android-tools/blob/master/LICENSE)
- [apktool](https://github.com/iBotPeaches/Apktool), licensed under the [Apache License 2.0](https://github.com/iBotPeaches/Apktool/blob/master/LICENSE.md)
- [erofs-utils](https://github.com/sekaiacg/erofs-utils/), dual license ([GPL-2.0](https://github.com/sekaiacg/erofs-utils/blob/dev/LICENSES/GPL-2.0), [Apache-2.0](https://github.com/sekaiacg/erofs-utils/blob/dev/LICENSES/Apache-2.0))
- [img2sdat](https://github.com/xpirt/img2sdat), licensed under the [MIT License](https://github.com/xpirt/img2sdat/blob/master/LICENSE)
- [platform_build](https://android.googlesource.com/platform/build/) (ext4_utils, f2fs_utils, signapk), licensed under the [Apache License 2.0](https://source.android.com/docs/setup/about/licenses)
- [smali](https://github.com/google/smali), [multiple licenses](https://github.com/google/smali/blob/main/third_party/NOTICE)

## Source and licensing

Impulse ROM is a modified fork of EternityROM.

Upstream:
https://github.com/Ocin4ever/EternityROM

Impulse changes:
[TomasULR/ImpulseROM](https://github.com/TomasULR/ImpulseROM), branch
[`bringup/oneui85-d2s`](https://github.com/TomasULR/ImpulseROM/tree/bringup/oneui85-d2s).
The initial public source snapshot is commit
[`a0728717`](https://github.com/TomasULR/ImpulseROM/commit/a0728717aab8bef2d42f4b0aee88f22defd002a2).
See [`docs/source-provenance.md`](docs/source-provenance.md) for the
limitations of matching this snapshot to the earlier Alpha 1 and Alpha 2 binaries.

The ROM build project is distributed under the GNU GPL v3 in
accordance with the upstream licence.

Linux kernel source:
see [`docs/kernel-source.md`](docs/kernel-source.md) — Impulse does not
modify kernel source; the prebuilt kernel package's own source
correspondence (including a currently-unresolved point) is documented there
rather than asserted here.

Kernel revision used by this release:
see [`docs/source-provenance.md`](docs/source-provenance.md) for the
per-release table.

KernelSU-Next revision:
see [`docs/kernel-source.md`](docs/kernel-source.md) — recorded, but not
proven to be exactly what was compiled into the distributed kernel binary
(explained there).

Samsung proprietary firmware components are external build inputs and
are not represented as original Impulse ROM source code. See
[`docs/proprietary-files.md`](docs/proprietary-files.md).

# Accountability
```cpp
#include <std_disclaimer.h>

/*
* Your warranty is now void.
*
* I am not responsible for bricked devices, dead SD cards,
* thermonuclear war, or you getting fired because the alarm app failed. Please
* do some research if you have any concerns about doing this to your device
* YOU are choosing to make these modifications, and if
* you point the finger at me for messing up your device, I will laugh at you.
*
* I am also not responsible for you getting in trouble for using any of the features in this ROM, including but not limited to Call Recording, secure flag removal etc.
*/
```

# Credits
A big thanks goes to the following for their invaluable contributions in no particular order (MORE INFO AND PEOPLE: TO BE WRITTEN)
- **[salvogiangri](https://github.com/salvogiangri)** for the UN1CA build system, OneUI patches, and general help and support while developing
- **[ExtremeXT](https://github.com/ExtremeXT)** for your support since the beginning and helping me with so many things. Special thanks to you!

Original ExtremeROM credits:
- **[Igor](https://github.com/BotchedRPR)** for getting me into porting, teaching me the basics, and emotional support down the road
- **[Halal Beef](https://github.com/halal-beef)** for lk3rd, testing and misc help
- **[Duhan](https://github.com/duhansysl)** for help with vendor backports, a lot of fixes and advice
- **[Anan](https://github.com/ananjaser1211)** for all of his contributions to OneUI porting
- **[PeterKnetch93](https://github.com/PeterKnetch93)** for help with smali and a lot of misc fixes
- **[tsn](https://github.com/tisenu100)** for some smali fixes and advice
- **[Nguyen Long](https://github.com/LumiPlayground)** for misc fixes and support
- **[Yagzie](https://github.com/Yagzie)** for engmode and misc fixes
- **[Fred](https://github.com/xfwdrev)** for WFD, HDR10+, audiopolicy and more fixes
- **[Saad](https://github.com/saadelasfur)** for help with build system
- **[Vince](https://github.com/vinceboberly)** for help with kernel upstream

Original UN1CA credits:
- **[ShaDisNX255](https://github.com/ShaDisNX255)** for his help, time and for his [NcX ROM](https://github.com/ShaDisNX255/NcX_Stock) which inspired this project
- **[DavidArsene](https://github.com/DavidArsene)** for his help and time
- **[paulowesll](https://github.com/paulowesll)** for his help and support
- **[Simon1511](https://github.com/Simon1511)** for his support and some of the device-specific patches
- **[ananjaser1211](https://github.com/ananjaser1211)** for troubleshooting and his time
- **[iDrinkCoffee](https://github.com/iDrinkCoffee-TG)** and **[RisenID](https://github.com/RisenID)** for documentation revisioning
- **[LineageOS Team](https://www.lineageos.org/)** for their original [OTA updater implementation](https://github.com/LineageOS/android_packages_apps_Updater)
- *All the UN1CA project contributors and testers ❤️*

# Stargazers over time
[![Stargazers over time](https://starchart.cc/Ocin4ever/EternityROM.svg)](https://starchart.cc/Ocin4ever/EternityROM)
