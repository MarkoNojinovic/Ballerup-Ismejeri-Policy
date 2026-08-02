# Ballerup-Ismejeri-Policy

Offentlige juridiske dokumenter for Ballerup Ismejeri-appen (GitHub Pages).

| Side | URL | Version |
|------|-----|---------|
| Privatlivspolitik | [`index.html`](https://markonojinovic.github.io/Ballerup-Ismejeri-Policy/) | 1.1 · 2. august 2026 |
| Handelsbetingelser | [`handelsbetingelser.html`](https://markonojinovic.github.io/Ballerup-Ismejeri-Policy/handelsbetingelser.html) | 1.2 · 2. august 2026 |
| Lejevilkår for isdisk | [`lejevilkaar.html`](https://markonojinovic.github.io/Ballerup-Ismejeri-Policy/lejevilkaar.html) | 2026-08 · 2. august 2026 |

## Sådan opdateres siderne

Kildedokumenterne bor i app-repoet `BI-New-iOS-Version` under `Legal/`:
`privatlivspolitik.md`, `handelsbetingelser.md` og `lejevilkaar-isdisk.md`.
HTML-siderne her er en spejling — **ret kilden først**, og overfør derefter ændringen hertil.

Bumpes en version væsentligt, skal `LegalPolicy.termsVersion` / `LegalPolicy.privacyVersion`
i kunde-appen (`Core/Legal/LegalPolicy.swift`) også bumpes. Det udløser gen-accept i appen.

**Lejevilkårene** kan redigeres af butikken i personale-appen (`config/iceDiskRentalTerms`
i Firestore). Sker det, er appens udgave den gældende — og `lejevilkaar.html` skal opdateres
manuelt, så de to ikke driver fra hinanden.

Den tidligere engelske politik fra 2024 er udgået og erstattet af siderne ovenfor.
