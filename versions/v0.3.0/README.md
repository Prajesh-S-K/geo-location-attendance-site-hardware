# v0.3.0 — Local release candidate

First complete, reviewable release: hardware-optional attendance, estimated room occupancy, optional Firebase mode, release tooling and honest documentation.

| | |
|---|---|
| Source | [`v0.3.0` in the main repository](https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026/tree/v0.3.0) (commit `cb2386f`) |
| Files in release | 101 |
| Change size | (baseline) |
| Download | `tech-pulse-0.3.0.zip` — see this repository's [Releases](https://github.com/Prajesh-S-K/geo-location-attendance-site-hardware/releases/tag/v0.3.0) |
| Size / SHA-256 | 1,518,324 bytes<br>`e86950c79782735e73b6d36fb521428b63bae370cb0f42a71055f6b863a3d0a0` |
| Automated checks | Node 92 · Chrome 11 · Firebase emulator 14 integration + 2 browser |

## What this version added or changed

- Defect fixes: live-database simulation endpoint removed; roster validation (existing students only, deduplicated, empty allowed, students cannot edit rosters); neutral advisory image similarity; review drawer driven by the latest attempt (missing reference, enlarge, expiry, completed states); inert map tooltips; Recorded / To review / Need action / Enrolled metrics; teacher session selector; shared confirmation dialogs; camera tracks stopped on leave/logout; sanitized browser storage.
- Proof policy per session: GPS + teacher review (default, no ESP32) or GPS + ESP32 classroom proof + teacher review; *Start replacement session without ESP32* with a shared attendance-event id so nobody is recorded twice.
- Estimated room occupancy (approved check-ins, check-outs, expiry) and a checks-and-anomalies panel.
- Optional Firebase Email/Password mode: ID-token to revocable server-session exchange, 8-hour cap from original sign-in, server-controlled roles, Firestore persistence with one transaction per approval, deny-all rules file.
- Launchers and tools: `demo`, `demo:connected`, `demo:phones`, `setup`, `doctor`, `firebase:init`, `deploy:web`, `release`; ESP32 upload pipeline with separate discovery / port / chip / compile / flash stages.
- Documentation rewritten to match the code; scanned, manifest-based release archive.

## Verified on real systems

Real project `tech-pulse-ssec`: owner provisioned, deny-all rules published and verified (client reads/writes 403), connected sign-in verified. ESP32 flashed (Wi-Fi network seen). HTTPS origin served on the Mac.

## Notes

Commit `53cddba` is the first release commit; `cb2386f` (tag v0.3.0) adds the real-project and hardware results to the docs. A repository bug (create operations overwriting existing attendance/presence documents) was found and fixed before this tag, with regression tests.

## Get exactly this version

```bash
git clone https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026.git
cd Tech_pulse-ssec-2026
git checkout v0.3.0
```
Or download `tech-pulse-0.3.0.zip`, extract it, open `README.md`.
