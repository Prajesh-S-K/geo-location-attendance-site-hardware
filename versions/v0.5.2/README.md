# v0.5.2 — Calmer phone launcher

Removed log noise from the phone launcher.

| | |
|---|---|
| Source | [`v0.5.2` in the main repository](https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026/tree/v0.5.2) (commit `a59dea8`) |
| Files in release | 114 |
| Change size | 6 files, +34/−22 vs v0.5.1 |
| Download | `tech-pulse-0.5.2.zip` — see this repository's [Releases](https://github.com/Prajesh-S-K/geo-location-attendance-site-hardware/releases/tag/v0.5.2) |
| Size / SHA-256 | 1,539,085 bytes<br>`b1150b68b85d513dc26ab6649d8ba321fde399be88442fd9cbf090dfb3d2de64` |
| Automated checks | Node 101 · Chrome 11 · Firebase emulator 14 + 2 |

## What this version added or changed

- The HTTPS proxy starts only after the server answers (no 'connection refused' spam).
- No Node TLS deprecation warning; phone launcher tests use real free ports.

## Verified on real systems

Run on the Mac: clean output.

## Notes

—

## Get exactly this version

```bash
git clone https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026.git
cd Tech_pulse-ssec-2026
git checkout v0.5.2
```
Or download `tech-pulse-0.5.2.zip`, extract it, open `README.md`.
