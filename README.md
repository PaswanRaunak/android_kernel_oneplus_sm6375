# OnePlus SM6375 kernel (msm-5.4 / holi) — PenguinOS

> **⚠️ BUILD STATUS: UNTESTED — NOT BOOT-VERIFIED.**
> Sources are configuration-audited (defconfigs verified, product graph
> resolves `TARGET_KERNEL_SOURCE`). No kernel build or device boot exists yet.

Linux **5.4** kernel for the OnePlus Nord CE 3 Lite 5G / Nord N30 5G
(qualcomm SM6375, platform `holi`), as used by LineageOS 24.0 and republished
for **PenguinOS `celerity`** builds.

## Build

Configured automatically by the build system
(`TARGET_KERNEL_SOURCE := kernel/oneplus/sm6375`):

- Defconfigs: `arch/arm64/configs/vendor/holi-qgki_defconfig` +
  `vendor/debugfs.config`
- Image: `Image` (arm64), boot header v3, DTB in bootimg, separated DTBO

## Provenance & licensing

- Based on Qualcomm/OnePlus **msm-5.4** sources (OnePlusOSS) with LineageOS
  integration patches; full Linux upstream history retained.
- Licensed **GPL-2.0** (see [`COPYING`](COPYING)). Distribution of any
  kernel binaries requires corresponding source availability — this
  repository fulfils that obligation for PenguinOS builds.

## Credits

- Linus Torvalds & Linux kernel contributors
- Qualcomm (qctecmdr) and OnePlus (OnePlusOSS) msm-5.4 sources
- LineageOS kernel team ( msm-5.4 maintenance and `lineage-24.0` integration)

## Known issues

- **Not boot-tested.** Kernel toolchain drift (PenguinOS clang vs the
  toolchain the LOS tree was validated with) may require flag adjustments
  on first build.

## Build status

```
[ UNTESTED / NOT BOOT-VERIFIED ]
Defconfig audit:     PASSED
Build:               NOT ATTEMPTED
Device boot:         NOT ATTEMPTED
```
