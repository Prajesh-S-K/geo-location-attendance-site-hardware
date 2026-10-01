# Tech Pulse — geo-fenced smart attendance: project record

The version-by-version record of **Tech Pulse (SSEC 2026)**, a geo-location attendance portal with an optional ESP32 classroom proof, optional Firebase accounts and private HTTPS for phones. Built for the Tech Pulse 2026 problem statement *Geo-Fenced Smart Attendance & Resource Management*.

- **Source code:** https://github.com/Prajesh-S-K/Tech_pulse-ssec-2026 (every version is a git tag)
- **This repository:** what each version is, what changed, how it was tested, the release zips (as GitHub Releases) with checksums, the project documents and screenshots.
- **Submitted version:** **v0.6.0**

## Versions

| Version | What it is | Automated checks | Download |
|---|---|---|---|
| [v0.3.0](versions/v0.3.0/README.md) | Local release candidate | Node 92 · Chrome 11 · Firebase emulator 14 integration + 2 browser | `tech-pulse-0.3.0.zip` |
| [v0.4.0](versions/v0.4.0/README.md) | One-command full launcher | Node 96 · Chrome 11 · Firebase emulator 14 + 2 | `tech-pulse-0.4.0.zip` |
| [v0.5.0](versions/v0.5.0/README.md) | Judge-friendly start | Node 99 · Chrome 11 · Firebase emulator 14 + 2 | `tech-pulse-0.5.0.zip` |
| [v0.5.1](versions/v0.5.1/README.md) | Quiet start, automatic Node selection | Node 101 · Chrome 11 · Firebase emulator 14 + 2 | `tech-pulse-0.5.1.zip` |
| [v0.5.2](versions/v0.5.2/README.md) | Calmer phone launcher | Node 101 · Chrome 11 · Firebase emulator 14 + 2 | `tech-pulse-0.5.2.zip` |
| [v0.6.0](versions/v0.6.0/README.md) | Big QR page and Windows full version (final) | Node 107 · Chrome 11 · Firebase emulator 14 + 2 | `tech-pulse-0.6.0.zip` |

Older history before v0.3.0 (local prototype, platform expansion, stabilization) is in [TIMELINE.md](TIMELINE.md). Integrity: [checksums/SHA256SUMS.txt](checksums/SHA256SUMS.txt).

## Repository layout

```
README.md            this page
STATUS.md            what is verified, what is not tested, what is pending
TIMELINE.md          project history in order
versions/vX.Y.Z/     one page per version (changes, evidence, checksum, how to get it)
docs/                project documents from the final version (architecture, evaluation, Firebase, phones, ESP32, demo, checklist, devlog, changelog)
screenshots/         synthetic-data screenshots of the final version
checksums/           SHA-256 of every release zip
```
Release zips are not stored in git; they are attached to each version's GitHub Release.

## Quick start (final version)

1. Install Node.js LTS (https://nodejs.org/).
2. Download `tech-pulse-0.6.0.zip` from the v0.6.0 Release and extract it.
3. Mac: right-click `Start Tech Pulse.command` → Open. Windows: double-click `Start Tech Pulse.bat`. Or run `npm run demo`.
4. The browser opens; a login list opens too. Details in the zip's `README.md`.

## Honest status

See [STATUS.md](STATUS.md). In short: software verified by automated tests (including Firebase emulators); real Firebase project, ESP32 flashing and the Mac HTTPS origin were exercised; **real phones, Windows and ESP32 power-cycle runs are not tested**.
