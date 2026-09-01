# Changelog

## 2.5.0 — 2026-09-01

- **New:** On-chain interval free-slot mode — `claimFree()` with no backend ticket (Cookiez style)
- **New:** Race mode toggle — broadcast immediately without simulation for pure-speed FCFS races
- **New:** Epoch-anchored slot timing — sync countdown to contract `mintOpenedAt` (Cookiez/Duh Goods)
- **Fix:** Simulate claimFree / freeMint before broadcast — never burn gas on a guaranteed-revert tx
- **Fix:** Retry simulation at slot boundary — catch the exact instant the slot opens
- **Fix:** Ticket freeMint simulation (struct EIP-712 + legacy)
- **Fix:** Cost Preview shows correct per-wallet USD instead of grand total

## 2.4.1 — 2026-08-25

- **New:** Desktop update check via GitHub Releases (banner + Settings section)
- **Fix:** Update check now points to the public blitzmint-releases repo
- **Fix:** Use reliable /releases?per_page=1 endpoint
- **Fix:** English-only UI strings in update section

## 2.4.0 — 2026-08-24

- **New:** License client integration (fingerprint, trial, gating, Settings tab)
- **New:** Ink network support (full OpenSea, gas tracker)
- **New:** Electron desktop app (portable .exe, fixed port 3420)
- **New:** Hardware fingerprint via node-machine-id (permanent trial)
- **New:** Portfolio sold detection via on-chain ownerOf
- **New:** CoinGecko price relay (wallet, calculator, cost preview)
- **New:** Snipe pre-auth for faster fire (hot refresh)
- **Fix:** Calculator gas format for cheap chains (Ink ~0.001 gwei)
- **Fix:** Free-slot double-start guard
- **Fix:** Mint-engine OpenSea relay path for unindexed ABI
- **Fix:** Trial mint reporting from SnipeEngine
