# v0.5.0 — Judge-friendly start

Made the project easy for a judge: extract, double-click, browser opens, logins listed.

| | |
|---|---|
| Source | [`v0.5.0` in the main repository](https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026/tree/v0.5.0) (commit `d4166a2`) |
| Files in release | 114 |
| Change size | 20 files, +537/−108 vs v0.4.0 |
| Download | `tech-pulse-0.5.0.zip` — see this repository's [Releases](https://github.com/Prajesh-S-K/geo-location-attendance-site-hardware/releases/tag/v0.5.0) |
| Size / SHA-256 | 1,536,433 (rebuilt from the tag) bytes<br>`5544c70e26eeae48a4aedd2b086eef188f978dc816adda9cc21db32ea7df2c68` |
| Automated checks | Node 99 · Chrome 11 · Firebase emulator 14 + 2 |

## What this version added or changed

- README rewritten as a judge guide with a five-minute walkthrough and troubleshooting table.
- Fast local start: `Start Tech Pulse.command` (Mac) and `Start Tech Pulse.bat` (Windows); browser opens by itself.
- `private/DEMO-LOGINS.txt`: every demo account, role, generated password and what to try (owner-only file).
- Phone setup page serving only the public CA (iPhone profile, Android certificate); launchers find Node by themselves.

## Verified on real systems

Fresh-extract acceptance run in a bare environment: install, build, start, login list written, one approved record, restart keeps data.

## Notes

The original 0.5.0 zip was overwritten by a later build on the maintainer's machine; the zip published here was rebuilt from the v0.5.0 tag with the same release script.

## Get exactly this version

```bash
git clone https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026.git
cd Tech_pulse-ssec-2026
git checkout v0.5.0
```
Or download `tech-pulse-0.5.0.zip`, extract it, open `README.md`.
