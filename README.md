# LineageOS 24.0 UNOFFICIAL — Galaxy M32 4G (SM-M325FV)

Unofficial LineageOS 24.0 (Android 17) for the Samsung Galaxy M32 4G. Vanilla, no GApps,
own signing keys, SELinux enforcing.

Latest: `lineage-24.0-20261117-UNOFFICIAL-m32` → [Releases](../../releases)

## Screenshots

| Setup | Trust | About phone |
|---|---|---|
| ![Setup wizard](docs/screenshots/Screenshot-20261117-171933-Setup-Wizard.png) | ![Trust](docs/screenshots/Screenshot-20261117-172227-LineageOS-Settings.png) | ![About phone](docs/screenshots/Screenshot-20261117-172255-Settings.png) |

## Fixed since last release

- SIM slot 2 data: DDS switch now falls back to the allow-data path, both slots get data
- Setup wizard: recovery-update and LineageOS consent pages removed, activities disabled
- No telemetry: stats collection off by default, legacy value reset on upgrade

## Removed

- Lineage recovery updater — TWRP stays on the recovery partition
- lineagestats (collector, services, wizard toggle)

## Install

1. Flash TWRP 3.6.11 (Mujammil, XDA 4800621) **together with the vbmeta disabler** in
   download mode (Odin: recovery in AP, vbmeta in USERDATA; heimdall: `--recovery` and
   `--vbmeta`) — one-time, otherwise the unsigned recovery will not boot
2. Coming from stock firmware only: flash `multidisabler.zip` once in TWRP — it removes
   Samsung's verity/force-encrypt flags. Not needed on later clean flashes or updates.
3. **Format Data**
4. Flash the zip from `/data/local/tmp`, reboot

Detailed steps (unlock, download mode, TWRP, clean flash) are in the m32f repository README
and apply the same way here.

**Never relock the bootloader** (hardbrick).

Credits: device trees [samsung-mt6768-aosp](https://github.com/samsung-mt6768-aosp), TWRP by Mujammil.
UNOFFICIAL build, no warranty.
