# Private XDA thread outline — Impulse ROM

> **Do not paste this text verbatim into XDA.** Current XDA Rule 15 says that
> AI-generated forum content is not permitted. Treat this document as a private
> factual outline and release checklist, rewrite the post in your own words, and
> verify every claim against the release build before publishing.

## Thread title

```text
[ROM][ALPHA][d2s][SM-N975F][Android 16] Impulse ROM v1.0 | One UI 8.5
```

## Private opening-post outline — XDA BBCode structure

```bbcode
[CENTER]
[SIZE=7][B]Impulse ROM[/B][/SIZE]
[SIZE=5]One UI 8.5 / Android 16 for the Galaxy Note10+ Exynos[/SIZE]

[B]Device:[/B] SM-N975F (d2s) only
[B]Current download:[/B] v1.0 One UI 8.5 Alpha 2 — test build, device testing pending
[B]Android:[/B] 16 / API 36
[B]Security patch:[/B] 5 June 2026
[B]SELinux:[/B] Enforcing
[/CENTER]

[COLOR=rgb(184, 49, 47)][SIZE=5][B]IMPORTANT WARNING[/B][/SIZE][/COLOR]

[B]Impulse ROM is an alpha release. It is intended for experienced users and secondary devices, not for a phone you depend on every day.[/B]

[LIST]
[*][B]SM-N975F / d2s Exynos only.[/B] Do not flash this on Snapdragon, Note10, Note10+ 5G or any other model.
[*]Unlocking the bootloader wipes the device and permanently trips the Knox e-fuse.
[*]Samsung Pay, Samsung Wallet and Knox-dependent features remain unavailable even after returning to stock.
[*]A public installation requires Format Data. Back up everything first.
[*]Keep verified stock Odin firmware, a working d2s TWRP image and an off-device EFS backup before flashing.
[*]You accept responsibility for data loss, broken applications or a non-booting device.
[/LIST]

[SIZE=5][B]About Impulse ROM[/B][/SIZE]

Impulse ROM brings the Galaxy S24 FE system base to the Exynos Galaxy Note10+, combining One UI 8.5 and Android 16 with the Note10+ vendor and hardware compatibility layer.

The project is a GPLv3 fork of EternityROM by Ocin4ever, built on the ROM build system created by Salvo Giangreco. It keeps the original authorship and copyright notices and adds d2s-specific compatibility, stability and installation safeguards.

[SIZE=5][B]Highlights[/B][/SIZE]

[LIST]
[*]One UI 8.5 based on Galaxy S24 FE firmware
[*]Android 16 / API 36 with the 5 June 2026 system security patch
[*]QHD+ 1440 x 3040 Note10+ display configuration
[*]SELinux enforcing
[*]ExtremeKRNL for d2s
[*]KernelSU-Next manager included — this build is rooted by design
[*]Package-scoped ROM signing; no unrestricted signature bypass
[*]Disabled incompatible Samsung OLED afterimage compensation; Alpha 2 still requires multi-day stability testing
[*]Photo Editor and camera changes included; Alpha 2 save/export and recording tests remain pending
[*]Extra dim SystemUI and Modes and Routines changes included; Alpha 2 device testing remains pending
[/LIST]

[SIZE=5][B]Previously tested functionality[/B][/SIZE]

The following describes earlier developer builds. Alpha 2 has not yet been flashed or runtime-tested according to its accompanying release notes, so all hardware features require retesting on this ZIP.

[LIST]
[*]System boot and normal UI
[*]Calls, SMS and LTE mobile data
[*]Wi-Fi and Bluetooth
[*]Speakers, earpiece, microphones and normal media audio
[*]Camera package present on the developer device; clean-install availability and photo/video capture remain unverified
[*]Fingerprint enrollment and unlock
[*]QHD+ display, touch and automatic brightness
[*]USB, ADB and MTP
[*]S Pen basics
[*]Wired charging
[/LIST]

[SIZE=5][B]Known issues[/B][/SIZE]

[LIST]
[*][B]Wireless charging does not work.[/B] The kernel interface is present, but the userspace cause has not yet been confirmed.
[*][B]Samsung Health refuses to start[/B] with the unauthorized-modifications / Knox-rooting error.
[*]Samsung Pay and Wallet are not supported. Secure Folder is reported working on Impulse; the next build still requires regression testing.
[*]Play Integrity fails. Some banking, work-profile and streaming applications may not run.
[*]Samsung camera AI, Gallery OCR and related NPU features are unstable. The Samsung snap service can restart when a model cannot be mapped.
[*]Alpha 2 includes Extra dim SystemUI and Modes and Routines provider changes, but their behavior has not yet been verified on the phone.
[*]Maximum outdoor brightness, HDR controls and Instagram/video playback require testing; these are not claimed as fixed.
[*]This release has not completed the full clean-install community test matrix. Please treat it as an alpha.
[/LIST]

[SIZE=5][B]Installation[/B][/SIZE]

[COLOR=rgb(184, 49, 47)][B]The following is only a summary. Read the complete installation guide before flashing.[/B][/COLOR]

[LIST=1]
[*]Download stock Odin firmware for your exact SM-N975F CSC and verify that it is complete.
[*]Back up all personal data and two-factor authentication credentials.
[*]Unlock the bootloader. This wipes the device and permanently trips Knox.
[*]Install a compatible d2s TWRP recovery and boot directly into recovery.
[*]Create an EFS backup and copy it away from the phone.
[*]In TWRP select Wipe -> Format Data and type yes. A normal factory reset is not enough.
[*]Copy the Impulse ROM ZIP to the phone, SD card or USB OTG storage.
[*]Verify the published SHA-256. Do not flash if it differs.
[*]Flash the ZIP and follow the on-screen confirmation. Do not interrupt filesystem resizing.
[*]Reboot. The first boot may take 10 to 20 minutes.
[/LIST]

[B]Dirty flashing from EternityROM 5.5 is unsupported. Use a clean installation with a complete backup; in-place migration has not been tested.[/B]

[SIZE=5][B]Download[/B][/SIZE]

[B]Download:[/B] [URL='https://drive.google.com/drive/folders/1BlQ1hBhLhhRsLkH6P1ozAfAJ7xOlbzKK?usp=drive_link']Impulse ROM — Google Drive[/URL]
[B]Alpha 2 files:[/B] [URL='https://drive.google.com/drive/folders/1vFBMG9UuvbmCtLBbB1dLnoBBvsxceyC6']v1.0-alpha2[/URL]
[B]Installation guide:[/B] [URL='https://drive.google.com/file/d/1MAffmzukrYESeZPal48-bqt_FkddgzQM/view?usp=drivesdk']INSTALL.md[/URL]
[B]Release status and known issues:[/B] [URL='https://drive.google.com/file/d/1sUQ1XYNcOMyJuh9KMnO7xTxLjt6NxAX7/view?usp=drivesdk']KNOWN_ISSUES.txt[/URL]
[B]Checksum file:[/B] [URL='https://drive.google.com/file/d/19UiWDayTD0BTfVOGM-QTYUr_uLViPnPz/view?usp=drivesdk']Alpha 2 SHA-256[/URL]

[B]Alpha 2 is a test build from an uncommitted working tree. Its accompanying release notes report offline validation, but no device boot or runtime testing. Clean-install validation remains incomplete.[/B]

[CODE]
File: ImpulseROM_v1.0-oneui85-alpha2_@c83e070e-dirty_20260901_d2s-sign.zip
Build date: 1 September 2026
Size: 5,800,045,146 bytes
SHA-256: 14cc19c811d4f0fcb39a429651fc26a17881eab4e233adbc38a9869cccf1504c
[/CODE]

[B]The flashable ZIP is not cryptographically signed. Always verify the SHA-256 after downloading.[/B]

[SIZE=5][B]Changelog — v1.0 Alpha 2[/B][/SIZE]

[LIST]
[*]Included Extra dim SystemUI and Modes and Routines provider changes; device testing pending
[*]Included Photo Editor and camera changes; save/export and recording tests pending
[*]Kept incompatible AfterimageCompensationService disabled
[*]Release notes report offline package, VINTF, audio, ELF32, ELF64 and ZIP integrity checks passing
[*]26 inherited non-critical patches remained at stock because they drifted against the Android 16 / One UI 8.5 source
[/LIST]

[SIZE=5][B]Previous changelog — v1.0 Alpha 1[/B][/SIZE]

[LIST]
[*]Initial Impulse ROM rebrand and d2s alpha release
[*]Galaxy S24 FE One UI 8.5 / Android 16 system base
[*]Disabled incompatible AfterimageCompensationService configuration responsible for recurring system soft reboots
[*]Updated Filter Provider to fix Samsung Photo Editor filter crashes
[*]Restored protected-content support required by Extra dim
[*]Hardened d2s recovery assertions and installation checks
[*]Added package-scoped Impulse platform signing
[*]Kept SELinux enforcing
[/LIST]

[SIZE=5][B]Source code and licences[/B][/SIZE]

[B]Impulse ROM source, including my changes:[/B] [URL='https://github.com/TomasULR/ImpulseROM']github.com/TomasULR/ImpulseROM[/URL]
[B]Source branch:[/B] [URL='https://github.com/TomasULR/ImpulseROM/tree/bringup/oneui85-d2s']bringup/oneui85-d2s[/URL]
[B]Initial public source snapshot:[/B] [URL='https://github.com/TomasULR/ImpulseROM/commit/a0728717aab8bef2d42f4b0aee88f22defd002a2']a0728717[/URL]
[B]Upstream EternityROM:[/B] [URL='https://github.com/Ocin4ever/EternityROM']github.com/Ocin4ever/EternityROM[/URL]
[B]Kernel source:[/B] [URL='https://github.com/Ocin4ever/ExtremeKernel/tree/f54c88ef6171ff3c4b5067911d5e8e4a0c62ec17']Ocin4ever/ExtremeKernel, v2.0 source tree[/URL]
[B]KernelSU-Next:[/B] [URL='https://github.com/KernelSU-Next/KernelSU-Next']github.com/KernelSU-Next/KernelSU-Next[/URL]
[B]Build instructions:[/B] [URL='https://github.com/TomasULR/ImpulseROM/blob/bringup/oneui85-d2s/BUILDING.md']BUILDING.md[/URL]
[B]Source and kernel provenance:[/B] [URL='https://github.com/TomasULR/ImpulseROM/blob/bringup/oneui85-d2s/docs/source-provenance.md']Release source records[/URL] | [URL='https://github.com/TomasULR/ImpulseROM/blob/bringup/oneui85-d2s/docs/kernel-source.md']Kernel source details[/URL]

The Impulse ROM build project and my modifications are distributed under GPLv3. The Linux kernel is GPLv2; external components retain their own licences. Samsung proprietary firmware blobs are build inputs and are not represented as original Impulse ROM work. Upstream authorship and copyright notices are preserved.

The public repository contains the accumulated Impulse changes. Alpha 1 and the September Alpha 2 test ZIP were built from uncommitted working trees, so the current public snapshot is not claimed to reproduce those ZIPs exactly. The unmodified prebuilt kernel is pinned to ExtremeKRNL v2.0; the exact KernelSU-Next driver commit compiled into it remains unverified because its upstream build used a floating submodule checkout. Kernel provenance and the Alpha 1 source limitations are documented in the source records linked above; Alpha 2's test status is recorded in its accompanying KNOWN_ISSUES.txt.

[SIZE=5][B]Credits[/B][/SIZE]

[LIST]
[*]Ocin4ever — EternityROM, from which Impulse ROM is forked
[*]Salvo Giangreco (@salvo_giangri) — original ROM build system
[*]ExtremeXT — ExtremeKRNL and Exynos kernel work
[*]rifsxd and the KernelSU-Next contributors — root solution
[*]Samsung — original firmware and device software
[*]Everyone testing and reporting issues with usable logs
[/LIST]

[SIZE=5][B]Bug reports[/B][/SIZE]

Before reporting a bug, reproduce it once and attach:

[CODE]
adb shell getprop ro.boot.em.model
adb shell getprop ro.build.version.security_patch
adb logcat -b all -d > logcat-all.txt
adb bugreport impulse-bugreport.zip
[/CODE]

Also include the exact ZIP filename, its SHA-256, whether you clean-flashed, and the steps that trigger the problem. Reports without logs may not be actionable.

[SIZE=5][B]Screenshots[/B][/SIZE]

[I]Attach current screenshots here: About phone, home screen, Settings, Quick Settings, Camera and Extra dim.[/I]

[CENTER][B]Flash carefully, keep a rollback path, and enjoy giving the Note10+ another life.[/B][/CENTER]
```

## Replace before publishing

- Verify anonymous download access to the supplied Drive folder and verify
  the ZIP against its checksum. The Alpha 2 checksum above is copied from
  its accompanying release notes/checksum file, not independently recomputed.
- Add current screenshots.
- Test Alpha 2 on the device, including Extra dim in Quick Settings,
  Accessibility and Modes and Routines. Record the actual results before
  changing its test status.
- The next new build needs a distinct version, exact source reference,
  filename, size and checksum; do not overwrite the September Alpha 2 ZIP.
- Perform at least one clean installation from the documented stock baseline.
- Capture a wireless-charger log and either fix the issue or retain the warning.
