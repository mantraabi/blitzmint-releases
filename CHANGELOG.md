# Changelog

## 2.7.3 — 2026-09-11

- **New:** Snipe hot-poll FCFS mode — polls OpenSea `swap()` from T−10s (400ms cadence, rate-limit safe), captures mint calldata the instant the stage flips, fires with zero relay round-trip. Built for Robinhood's ~100ms blocks after the RPG Genesis Chest postmortem
- **New:** Early-fire — when every selected wallet's calldata is captured, the phase fires immediately instead of waiting for the target time
- **New:** Hot-poll toggle in snipe controls (default ON, OpenSea drops only)
- **Fix:** Robinhood RPC fallback — added `rpc.ordofi.network` (blockscout eth-rpc now 403); effective order: custom → Alchemy → publicnode → ordofi

## 2.7.2 — 2026-09-09

- **Fix:** Contract-mint price detection for custom views (`publicPrice()`, `mintFee()`, `mintCost()`, `salePrice()`) — value auto-fills on paid mints
- **Fix:** False "reverts" badge on paid contract mint (payable re-probe with the detected price)

## 2.7.1 — 2026-09-09

- **New:** Arc (5042002) registered as inactive chain
- **Fix:** Wallet import success toast + auto-close modal

## 2.7.0 — 2026-09-09

- **Removed:** Free Slot Mint (engine, page, relay) and NFT Portfolio (NFTs page, PnL cards) — app focuses on Mint OpenSea · Mint Contract · Wallets
- Activity-log `nft_received` entries kept; `extractMintedNfts` retained for receipt parsing

## 2.6.0 — 2026-09-09

- **Removed:** License system (fingerprint, trial, gating) — the app is now completely free
- **New:** Settings → Support (donate) tab
- **New:** Manual signature mint for unverified-ABI contracts (eth_call probe + executor)

## 2.5.0 — 2026-09-01

- On-chain interval free-slot mode `claimFree()` (removed again in 2.7.0)

## 2.4.1 — 2026-08-25

- Desktop update check via GitHub Releases (banner + Settings section)

## 2.4.0 — 2026-08-24

- License client, Ink network support, Electron portable .exe, CoinGecko price relay, snipe pre-auth at T−2s
