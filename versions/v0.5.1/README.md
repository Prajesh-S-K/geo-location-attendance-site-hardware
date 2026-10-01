# v0.5.1 — Quiet start, automatic Node selection

Fixed a reported first-run experience: a red 'Node too old' error and a wall of npm warnings.

| | |
|---|---|
| Source | [`v0.5.1` in the main repository](https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026/tree/v0.5.1) (commit `bc5bac6`) |
| Files in release | 114 |
| Change size | 10 files, +208/−48 vs v0.5.0 |
| Download | `tech-pulse-0.5.1.zip` — see this repository's [Releases](https://github.com/Prajesh-S-K/geo-location-attendance-site-hardware/releases/tag/v0.5.1) |
| Size / SHA-256 | 1,538,886 bytes<br>`f92cb85d0baaee27bf371b17fc2b3e04daf5bd770554441699c00b9cb1ea000e` |
| Automated checks | Node 101 · Chrome 11 · Firebase emulator 14 + 2 |

## What this version added or changed

- If the default Node is too old but a newer one is installed (nvm/Homebrew), the launcher continues with it automatically; otherwise a three-step plain message.
- Install and build output hidden unless something fails; three numbered steps (Step 1 of 3 … Step 3 of 3).
- README start steps rewritten for first-time users.

## Verified on real systems

Reproduced with the old default Node 22.9 first on PATH: clean three-step start.

## Notes

—

## Get exactly this version

```bash
git clone https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026.git
cd Tech_pulse-ssec-2026
git checkout v0.5.1
```
Or download `tech-pulse-0.5.1.zip`, extract it, open `README.md`.
