# v0.6.0 — Big QR page and Windows full version (final)

Final submitted version: phone setup by large on-screen QR codes, and the full phone version on Windows.

| | |
|---|---|
| Source | [`v0.6.0` in the main repository](https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026/tree/v0.6.0) (commit `32c0f97`) |
| Files in release | 118 |
| Change size | 17 files, +394/−54 vs v0.5.2 |
| Download | `tech-pulse-0.6.0.zip` — see this repository's [Releases](https://github.com/Prajesh-S-K/geo-location-attendance-site-hardware/releases/tag/v0.6.0) |
| Size / SHA-256 | 1,545,120 bytes<br>`387099b36624d859ecc17720e9e590b64732364fb2b2608f63064dbac9b84a45` |
| Automated checks | Node 107 · Chrome 11 · Firebase emulator 14 + 2 |

## What this version added or changed

- Browser page with two large black-on-white QR codes (certificate, then app) plus typeable addresses; verified by decoding a screenshot with macOS Vision.
- `Start Tech Pulse with Phones.bat` and `Stop Tech Pulse.bat`; winget installs mkcert/Caddy; Windows process detection for stopping older copies; Windows-safe Caddyfile paths.
- Automatic choice of the real Wi-Fi address (ignores WSL/VPN/VirtualBox adapters).

## Verified on real systems

Run on the Mac: both QR codes decode to the correct addresses; certificate page serves the public CA only (private key request returns 404).

## Notes

Windows support is unit-tested with Windows-shaped input; it has not been run on a Windows machine.

## Get exactly this version

```bash
git clone https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026.git
cd Tech_pulse-ssec-2026
git checkout v0.6.0
```
Or download `tech-pulse-0.6.0.zip`, extract it, open `README.md`.
