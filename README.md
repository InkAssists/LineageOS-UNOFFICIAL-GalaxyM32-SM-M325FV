# LineageOS 24.0 UNOFFICIAL — Galaxy M32 4G (SM-M325FV, EU)

Unofficial LineageOS 24.0 (Android 17) for **SM-M325FV (`m32`) only**. Do not cross-flash the India SM-M325F build; the shared recovery assertion does not distinguish the two models.

## Downloads and installation

- [Releases](../../releases) — ROM ZIPs and checksums
- [Installation guide](INSTALL.md) — bootloader, TWRP, and clean flash

## What's working

- The 2026-11-24 EU test build boots after a clean flash.
- Mobile data on both SIM slots was verified on the previous EU release (2026-11-17); not independently reverified on this build.
- Standby with AOD off: about one battery percentage point lost overnight in a tester observation, not a controlled measurement.

## Known issues on the 2026-11-24 test build

- The visible Always-On Display clock can freeze at the time the phone was locked. Disabling AOD is a workaround.
- Leaving AOD on increases standby battery drain, even in airplane mode. **We recommend turning AOD off for better battery life.**
- The lock screen may show a 12-hour clock despite the expected 24-hour format.

## Screenshots (2026-11-17)

| Setup | Trust | About phone |
|---|---|---|
| ![Setup wizard](docs/screenshots/Screenshot-20261117-171933-Setup-Wizard.png) | ![Trust](docs/screenshots/Screenshot-20261117-172227-LineageOS-Settings.png) | ![About phone](docs/screenshots/Screenshot-20261117-172255-Settings.png) |

## Credits

Device trees: [samsung-mt6768-aosp](https://github.com/samsung-mt6768-aosp). TWRP: Mujammil.
