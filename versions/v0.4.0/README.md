# v0.4.0 — One-command full launcher

Replaced the multi-step phone/Firebase routine with a single command.

| | |
|---|---|
| Source | [`v0.4.0` in the main repository](https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026/tree/v0.4.0) (commit `be4c4e6`) |
| Files in release | 107 |
| Change size | 14 files, +447/−6 vs v0.3.0 |
| Download | `tech-pulse-0.4.0.zip` — see this repository's [Releases](https://github.com/Prajesh-S-K/geo-location-attendance-site-hardware/releases/tag/v0.4.0) |
| Size / SHA-256 | 1,527,099 bytes<br>`90531f6d0b23080fbe9c7cf329b71fbbb1da1cec0885c7628cc7f4048b936f81` |
| Automated checks | Node 96 · Chrome 11 · Firebase emulator 14 + 2 |

## What this version added or changed

- `npm run full` and double-click `Start Tech Pulse.command` / `Stop Tech Pulse.command`.
- Stops older Tech Pulse processes started from the same folder (never unrelated programs).
- Validates Firebase configuration first; installs mkcert/Caddy with Homebrew; creates the local CA once; copies the public certificate to Downloads and reveals it; picks free ports.
- `npm run stop`.

## Verified on real systems

Run for real on the Mac: a second launch stopped the 4 older processes and started cleanly; the page loaded over HTTPS with the mkcert CA.

## Notes

Terminal QR codes were introduced here (later replaced in v0.6.0).

## Get exactly this version

```bash
git clone https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026.git
cd Tech_pulse-ssec-2026
git checkout v0.4.0
```
Or download `tech-pulse-0.4.0.zip`, extract it, open `README.md`.
