# LineageOS 24.0 UNOFFICIAL — Galaxy M32 4G (SM-M325FV)

Unofficial LineageOS 24.0 (Android 17) builds for the Samsung Galaxy M32 4G (SM-M325FV, mt6768 / Helio G80).

**SELinux runs ENFORCING (since build 2026-11-13). Widevine L3 only (SD streaming works; L1 is permanently lost after bootloader unlock). Play Integrity will not pass (unlocked bootloader).**

- Downloads: see [Releases](../../releases)
- Device trees: [samsung-mt6768-aosp](https://github.com/samsung-mt6768-aosp) (ArtZabAZ)
- Recovery: TWRP 3.6.11 by Mujammil (XDA thread 4800621)
- Flash: TWRP + `multidisabler` + **Format Data** + flash zip. **NEVER relock the bootloader** (hardbrick).

Known issues:
- Harmless SELinux log spam (dmabuf denials) while rendering — fix planned.
- Widevine L1 unavailable (L3 only) — inherent to unlocking a Samsung device (Knox keybox), not fixable.

No warranty of any kind.