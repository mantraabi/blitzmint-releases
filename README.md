# BlitzMint — NFT Mint Bot for EVM Chains

**BlitzMint** is a fast, focused NFT mint bot for EVM-compatible chains (Ethereum, Base, Ink, Robinhood, Polygon, Arbitrum, Optimism, BNB Chain, Avalanche, Arc, and more). Snipe OpenSea drops at stage-open precision, mint from any verified contract, and manage multi-wallet batches — all with 100% client-side custody.

**BlitzMint** adalah bot NFT mint untuk jaringan EVM yang dirancang untuk kecepatan dan presisi. Cocok untuk kolektor, trader, dan pemburu NFT yang ingin mengotomatiskan minting dengan fitur snipe OpenSea drop, mint contract, dan dukungan multi-wallet.

> **100% client-side custody** — private keys and wallet vault live in your browser. The local server is only a relay (RPC/proxy/OpenSea); keys never leave your machine.

---

## 🔑 Key Features / Fitur Utama

| English | Indonesia |
|---------|-----------|
| **Snipe Engine** — multi-phase scheduling (WL → GTD → FCFS → Public) with T−2s hot refresh and OpenSea pre-auth | **Snipe Engine** — jadwal multi-phase (WL → GTD → FCFS → Public) dengan hot refresh T−2s dan pre-auth OpenSea |
| **Hot-poll FCFS Mode** — polls OpenSea `swap()` from T−10s and fires the instant the stage opens — built for Robinhood's ~100ms blocks | **Hot-poll FCFS** — polling `swap()` OpenSea dari T−10s dan langsung nembak detik stage kebuka — dibuat untuk block ~100ms Robinhood |
| **Mint OpenSea** — full drop lookup: stages, prices, per-wallet caps, batch eligibility across vault wallets | **Mint OpenSea** — lookup drop lengkap: stage, harga, cap per wallet, batch eligibility lintas wallet |
| **Mint Contract** — verified-ABI encoding, custom views (`publicPrice()`, `mintFee()`, …), eth_call probe for unverified contracts | **Mint Contract** — encoding ABI verified, custom view functions, probe `eth_call` untuk kontrak unverified |
| **Multi-Wallet Vault** — encrypted local vault; mint/fund/withdraw across many wallets with per-wallet proxies | **Multi-Wallet Vault** — vault terenkripsi lokal; mint/fund/withdraw multi-wallet dengan proxy per-wallet |
| **Safety Guards** — Free Mint Guard (free→paid flip protection), simulation-first broadcast, per-wallet readiness checks | **Safety Guards** — Free Mint Guard (deteksi free→paid), simulasi sebelum broadcast, readiness check per wallet |
| **RPC Manager** — custom RPC priority, Alchemy support, automatic failover (Robinhood: publicnode + ordofi) | **RPC Manager** — prioritas custom RPC, dukungan Alchemy, failover otomatis (Robinhood: publicnode + ordofi) |
| **Gas Calculator + Cost Preview** — live per-wallet cost estimates before you commit | **Kalkulator Gas + Cost Preview** — estimasi biaya per wallet sebelum eksekusi |
| **Desktop App** — portable Windows .exe, runs locally, auto-update via GitHub Releases | **Aplikasi Desktop** — portable .exe Windows, berjalan lokal, auto-update via GitHub Releases |

### Removed in 2.7.0 / Dihapus di 2.7.0

Free Slot Mint and NFT Portfolio were removed to keep the app focused on what matters: **Mint OpenSea · Mint Contract · Wallets**. Activity-log entries for received NFTs are kept.

Free Slot Mint dan Portfolio NFT dihapus supaya app fokus ke yang benar-benar dipakai: **Mint OpenSea · Mint Contract · Wallets**. Catatan NFT di Activity Log tetap ada.

---

## 📥 Download / Unduh

> **Latest Release:** [v2.7.5](https://github.com/mantraabi/blitzmint-releases/releases/latest)
>
> Download `BlitzMint-2.7.5-portable.exe` — portable, no installation required.
> No admin rights needed. Just download and run.

**System Requirements:**
- Windows 10 / 11 (64-bit)
- Internet connection (for RPC and API calls)
- No installation — portable .exe, runs from any folder

---

## 🚀 Quick Start

1. [Download the latest .exe](https://github.com/mantraabi/blitzmint-releases/releases/latest)
2. Run `BlitzMint-2.7.5-portable.exe`
3. Import your wallet via private key or seed phrase (stored encrypted, locally)
4. **Mint OpenSea**: paste a drop contract address → check stages → execute or snipe
5. **Mint Contract**: paste any contract → detected mint function → execute or snipe
6. (Optional) Add an Alchemy API key in Settings → API Keys, then pick Alchemy in Settings → RPC for the fastest, freshest blocks

---

## 🔗 Links / Tautan

- **Documentation / Panduan:** [blitzmint-docs.vercel.app](https://blitzmint-docs.vercel.app)
- **Changelog / Riwayat Versi:** [CHANGELOG.md](./CHANGELOG.md)

---

## 💚 Free & Open / Gratis

BlitzMint is **free to use** — no license keys, no trial limits. All mint/snipe features are unlimited. If the app helps you, support development via **Settings → Support** (donation).

BlitzMint **gratis penuh** — tanpa kunci lisensi, tanpa batas trial. Semua fitur mint/snipe unlimited. Kalau app-nya membantu, dukung pengembangan lewat **Settings → Support** (donasi).

© 2026 Abi Creative — [abicreative.web.id](https://abicreative.web.id)
