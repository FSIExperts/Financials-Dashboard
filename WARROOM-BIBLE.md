# ⚡ WAR ROOM BIBLE — Anne's Portfolio
**Last Updated:** February 26, 2026  
**File naming standard:** `WARROOM-BIBLE.md` — always this name, always overwrite with latest.

---

## 🗂 CONTEXT

This is an IRA brokerage account (not taxable). Investment focus: **AI infrastructure boom** across two themes — Semiconductors/Chips and Energy/Power. Secondary positions in defense, aerospace, finance, space.

**Brokerage:** Fidelity (based on order screenshots)  
**Dashboard file:** `portfolio-monitor.html` — single-file static app, deployed to github.io  
**Monopoly App:** Separate project — rental property tracker with Monopoly-style interface. 104 Court is a real property. Discussed but not yet built.

---

## ✅ COMPLETED TRADES (This Session)

| Trade | Details |
|-------|---------|
| ETHU sold | 25 shares @ $23.02 market order, Feb 25 2026 |
| IBIT sold | 25 shares market order (cleaned up crypto ETFs together) |
| NVDL triggered | 50 shares, stop-limit $85/$82 GTC triggered Feb 26 |
| CRWD added | 5 shares @ $380.29 → now 10 shares total |

**Rationale for crypto cleanup:** Sold IBIT and ETHU (leveraged ETF) from IRA — no leverage decay, no crypto in IRA. Still holds ETH and SOL directly on Coinbase (~$3,500 ETH, ~$1,000 SOL) — keeping those, too small to matter and own the actual assets.

---

## 🟡 OPEN ORDERS (Active Right Now)

| Ticker | Order | Details | Status |
|--------|-------|---------|--------|
| SNOW | Limit Sell | 10 shares @ $172.00 GTC exp 08/24/2026 | OPEN |
| NVDA | Stop-Limit Sell | 50 shares, Stop $171 / Limit $169 GTC exp 02/27/2026 | OPEN ⚠️ EXPIRES SOON |
| NFLX | Stop-Limit Sell | 45 shares, Stop $72 / Limit $70 GTC exp 08/21/2026 | OPEN |

**⚠️ NVDA stop expires 02/27/2026 — RENEW IMMEDIATELY or it lapses.**

**SNOW plan:** 10 shares at $172 GTC open. When that fills → sell remaining 10 shares immediately. Exit completely. Securities class action lawsuit filed + ex-CEO sold 100K shares pre-earnings. Take the profit.

---

## 💼 FULL PORTFOLIO

### Watch / Active Risk Positions

| Ticker | Shares | Cost* | Stop | Target | Verdict | Notes |
|--------|--------|-------|------|--------|---------|-------|
| NVDA | 50 | $140 | $171/$169 | $200 | STOP ACTIVE | Touched $171 Feb 26, bounced — confirmed support. Renew stop. |
| SNOW | 20 | $145 | — | $172 | ⚠️ EXIT | Lawsuit + insider sale. Sell all at $172. |
| NFLX | 45 | $78 | $72/$70 | $125 | TRADE | WBD deal + DOJ probe. Reversion trade only. |

### Core Holdings

| Ticker | Shares | Cost* | Target | Verdict | Thesis |
|--------|--------|-------|--------|---------|--------|
| AVGO | 25 | $185 | $414 | STRONG HOLD | AI custom chips doubling 2026, $73B backlog, pays dividend |
| AMD | 18 | $155 | $267 | HOLD | AI GPU #2, MI300X enterprise traction |
| CRWD | 10 | $350 | — | HOLD | AI cybersecurity, added 5 @ $380.29 |
| LRCX | 15 | $180 | — | HOLD | Chip equipment, BofA top pick |
| XOM | 51 | $108 | $157 | HOLD | Energy ballast, 3.5% dividend, AI gas demand |
| ET | 750 | $13.50 | — | STRONG HOLD | Largest position, 7-8% distribution, AI data center gas pipelines |
| HWM | 20 | $95 | $320 | STRONG HOLD | Hit ATH $256, JPM $320 target, let it run |
| AME | 25 | $155 | — | HOLD | Industrial AI automation, compounder |
| DE | 15 | $380 | — | HOLD | AI-guided autonomous farming |
| JPM | 25 | $195 | — | HOLD | Best bank, AI-resistant moat, growing dividend |
| AVAV | 30 | $195 | $320 | HOLD | Defense drones + AI, JPM Overweight $320 |
| RKLB | 125 | $12 | — | WATCH | Neutron rocket catalyst, volatile |
| RKT | 300 | $11.50 | $22 | HOLD | Rate play, Redfin + Mr Cooper |
| TSLA | 20 | $250 | — | WATCH | Optimus + FSD thesis, Musk risk |
| AG | 550 | $7.50 | — | HOLD | Silver miner, solar/EV industrial demand |

*Cost basis = Jan 1 2026 placeholder. Update with real data.

---

## 💰 CASH & DEPLOY PLAN

**Estimated IRA Cash:** ~$12,000+  
Sources: ETHU proceeds + IBIT proceeds + NVDL proceeds + existing $7,752 cash

### Deploy Priority Order

| Ticker | Amount | Why |
|--------|--------|-----|
| NVDA | ~$3,500 | Add ~20 shares on dip to $175-182. Own real shares not leveraged ETF. |
| CEG | ~$2,500 | Constellation Energy. Largest nuclear operator + Microsoft 20yr AI power deal. ~20% off highs. |
| VST | ~$2,500 | Vistra. 2nd largest nuclear fleet. Same AI power demand thesis. |
| MU | ~$2,000 | Micron. HBM memory. Completes chip supply chain. Morgan Stanley #1 semi pick 2026. |
| GEV | ~$1,500 | GE Vernova. Power infrastructure. $2B direct DC orders. 71% EPS growth FY26. |

Add SNOW proceeds (~$3,440 if fills at $172) to the pool — pushes total toward ~$15K+.

---

## 📅 UPCOMING ACTIONS

- [ ] **URGENT:** Renew NVDA stop-limit — expires 02/27/2026. Reset to $178/$176 if price stable above $185.
- [ ] Enter SNOW limit sell for remaining 10 shares once first 10 fills at $172.
- [ ] Check RKLB earnings result — Neutron rocket update is key signal.
- [ ] Check RKT earnings result — watch mortgage origination volume.
- [ ] Begin deploying cash — NVDA dip first, then CEG/VST/MU/GEV.
- [ ] Update WARROOM-BIBLE with real cost basis when available.

---

## 🛠 TECH / TOOLS

### portfolio-monitor.html
- Single HTML file, deploys to github.io as-is
- Uses Finnhub free API (user pastes key, saved to localStorage)
- Falls back to corsproxy.io → Yahoo Finance if no key
- Chart.js 4.4.1 from CDN for price charts
- Features: sticky nav, alert system, cards with risk color coding, full table with P&L, search + chart, deploy plan
- **Next upgrade path:** When outgrowing static github.io → move to Vercel/Netlify with a Node backend for real-time WebSocket prices, push alerts, and persistent storage

### File Naming Convention
- Dashboard: `portfolio-monitor.html`
- This bible: `WARROOM-BIBLE.md`
- Playbook (full position thesis doc): `Anne_Portfolio_Playbook.docx`

---

## 🎯 INVESTMENT THESIS SUMMARY

**AI Infrastructure Boom — Two Pillars:**

1. **Chips/Semis** — NVDA (GPU king), AVGO (custom AI chips), AMD (#2 GPU), LRCX (equipment). Missing: MU (memory) — deploy soon.

2. **Power/Energy** — ET + XOM (existing). Missing nuclear: CEG + VST. Missing infrastructure: GEV. These are the "picks and shovels" of AI data center power demand. Hyperscalers spending $600B+ capex in 2026.

**AI-Resistant Moats (supporting positions):** JPM (regulatory), CRWD (security), HWM (aerospace supply chain), AVAV (defense).

**Key Risk to Monitor:** If hyperscalers signal AI capex pullback → chips and energy positions get hit hard. Watch quarterly guidance from MSFT/GOOGL/AMZN/META.

---

## 🏠 MONOPOLY APP (Separate Project)

**Concept:** Rental property tracker with Monopoly-style visual interface.  
**104 Court** = real rental property (the "green house" reference).  
**Features planned:** Property cards like Monopoly board, rent tracking, expense tracking, equity display, "collect rent" when someone pays.  
**Status:** Concept only, not yet built. Start in a fresh chat with this bible for context.

---

*Paste this file at the start of any new chat session to restore full context.*
