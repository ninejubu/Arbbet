# Alpha Leak

Self-contained HTML calculators for the **Spot + Long Put + Bet NO** strategy
(always-positive return at any settlement price) and **Cash & Carry**, with live
market data.

## Files

| File | What it does |
|---|---|
| `index.html` | **Main dashboard** (served at the site root) — 3 tabs: **Arbbet** (Spot + Put + NO), **Cash & Carry** (spot + 1x short delivery), **Info** (explanations & examples). |
| `alpha_leak_ep1_spot_put_no.html` | Standalone version of the Spot + Put + NO calculator. |
| `alpha_leak_ep2_cash_and_carry.html` | Standalone version of the Cash & Carry calculator. |

## Data sources

- **ETH / BTC** — Bybit (cash-settled USDT options, exp 25 DEC 26) via `api.bytick.com` (v5 API)
- **Gold** — Deribit PAXG spot + embedded GLD (Webull) options snapshot
- **NO bets** — Polymarket (gamma API), settles 31 DEC 26

All figures are per **$1,000** of capital, net of trading fees
(Bybit options fee: 0.03% of underlying, capped at 12.5% of premium;
spot 0.1% per trade; Polymarket taker fee).

Open any file directly in a browser — no build step, no server.
