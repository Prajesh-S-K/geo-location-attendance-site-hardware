# Status of the final version (v0.6.0)

## Verified by automated tests
- 107 Node tests (rules, API, launchers, Windows-shaped inputs, tooling, persistence, occupancy, concurrency, release scan).
- 11 Chrome tests (review drawer, expiry, policy/replacement, occupancy and check-out, anomalies, maps, three phone widths, permissions).
- Firebase emulators: 14 integration tests and 2 browser tests (authorization, atomic approval, persistence failure, restart, replacement chain, deny-all rules, real UI sign-in/renewal/logout).
- Release archive: manifest-based, scanned for secrets and machine paths (0 findings); fresh-extract acceptance runs.

## Exercised on real systems
- Real Firebase project: owner provisioned, deny-all Firestore rules published and verified (anonymous and signed-in client access return 403), connected sign-in and session exchange verified.
- ESP32 (plain ESP32-D0WD-V3, 4MB) identified read-only, flashed, and its Wi-Fi network observed.
- Private HTTPS origin and certificate page served on the Mac; both QR codes decode to the right addresses.

## Not tested
- A real iPhone or Android phone scanning the codes and completing a check-in.
- Running anything on an actual Windows machine.
- ESP32 on standalone power / after a power cycle; serial readiness lines were not captured.
- A full attendance cycle on the real Firebase project with real students.
- Battery consumption (design: one-shot location, camera tracks stopped; no measurement).

## Pending on the owner
- Real-device acceptance above; replace illustrative venue coordinates with the real room; licence choice.

## Not included here (by design)
Credentials, Admin keys, owner passwords, real student data, photos, generated firmware secrets. They live only in the owner's private folder.
