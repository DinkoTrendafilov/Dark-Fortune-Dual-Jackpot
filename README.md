# 🎰 Dark Fortune — Dual Progressive Jackpot Slot

> A mathematically rigorous slot game model featuring an original dual progressive jackpot mechanism, validated through 10,000,000 Monte Carlo simulation iterations.

---

## 🎮 Play the Live Demo

**👉 [Click here to play Dark Fortune](https://dinkotrendafilov.github.io/Slot-Machine-Dual-Jackpot/DEMO_dark_fortune_dual_jackpot.html)**

No installation needed. Just click and play!

---

## 📌 Project Overview

**Dark Fortune** is a custom-designed slot game built from scratch, combining combinatorial probability theory, progressive jackpot design, and survival analysis. The project includes a full Python mathematical model and a playable HTML5 demo.

| Parameter | Value |
|-----------|-------|
| Reels | 5 |
| Rows | 4 |
| Paylines | 20 |
| Symbols | 30 unique |
| Total combinations | 24,300,000 |
| Target RTP | 95.001% |
| Achieved RTP (10M sims) | **96.16%** |
| Zero-win spins | **0.00%** |

---

## 💡 Original Mechanism — What Makes This Different

Most slot games pay out for **2+ matching symbols** on a payline. Dark Fortune introduces a novel approach:

- **1-of-5 match** → pays **0.5×** the line bet directly (occurs ~70% of all lines)
- **2-of-5 match** → feeds **both jackpot pools** (occurs ~28.5% of all lines)
- **3-of-5 match** → pays **10×** the line bet
- **4-of-5 match** → pays **900×** the line bet
- **5-of-5 match** → pays **50,000×** the line bet

This design ensures **zero-win spins are statistically impossible** — validated across 10,000,000 spins. Every spin returns something, maximizing player engagement and session time.

---

## 💎 Dual Progressive Jackpot System

Two independent jackpot pools are organically fed by 1-match and 2-match lines:

| Jackpot | Trigger Probability | RTP Contribution | Avg Payout |
|---------|--------------------|--------------------|------------|
| 🔵 Blue Jackpot | 1 in 300 | 2.69% | ~161 credits |
| 💜 Grand Jackpot | 1 in 3,000 | 2.86% | ~1,685 credits |
| **Combined** | — | **5.55%** | — |

**Key design principle:** Jackpot pools are funded by lines that would otherwise pay nothing — making the accumulation completely organic and tied to real game activity, not an artificial tax on the player's bet.

Both jackpots trigger **independently** on each spin, meaning both can theoretically trigger on the same spin.

---

## 📊 RTP Distribution

| Group | Probability | Coefficient | RTP Contribution |
|-------|-------------|-------------|------------------|
| 1 match | 70.37% | 0.5× | 38.79% |
| 2 match | 28.57% | 0.8× | 25.20% |
| 3 match | 1.04% | 10× | 11.45% |
| 4 match | 0.018% | 900× | 17.76% |
| 5 match | 0.0001% | 50,000× | 6.81% |
| 🔵 Blue Jackpot | 1:300 | progressive | 2.69% |
| 💜 Grand Jackpot | 1:3000 | progressive | 2.86% |
| **Total** | | | **96.16%** |

---

## 🧮 Mathematical Model

### Combinatorial Analysis
All 24,300,000 possible 5-reel combinations are enumerated exhaustively (30^5). Each combination is classified by maximum matching symbol count, enabling exact theoretical RTP calculation.

### Monte Carlo Validation
- **10,000,000 spin simulation**
- Blue Jackpot hits: **33,354** (avg every 300 spins, theoretical: 300) ✅
- Grand Jackpot hits: **3,395** (avg every 2,946 spins, theoretical: 3,000) ✅

### Bayesian Analysis — 5-of-5 Frequency
- Theoretical: 1 in 40,500
- Simulated: 1 in 40,984
- 95% Credible Interval: [1 in 36,151 — 1 in 46,451]
- ✅ Theoretical probability is within 95% CI

---

## 💀 Survival Analysis (Bankroll Simulation)

**Setup:** 1,000 sessions, 10,000 initial credits, 20 credits per spin (1 credit × 20 lines)

| Spins | Survival Rate | Bust Rate | Avg Balance | Avg Survivor Balance |
|-------|--------------|-----------|-------------|---------------------|
| 500 | **100.00%** | 0.00% | 9,705 | 9,705 |
| 1,000 | **100.00%** | 0.00% | 9,359 | 9,359 |
| 2,000 | **97.90%** | 2.10% | 8,792 | 8,980 |
| 5,000 | 43.70% | 56.30% | 7,579 | 17,324 |
| 10,000 | 13.10% | 86.90% | 6,150 | **46,841** |

**Notable insight:** Players who survive 10,000 spins average **46,841 credits** — a **+368% return** on initial capital. This is the characteristic behavior of a progressive jackpot game: most players experience gradual decline, while jackpot winners achieve exceptional returns.

---

## 📈 Volatility Profile

| Metric | Value |
|--------|-------|
| Standard Deviation (σ) | 294.38 |
| Arithmetic Mean (μ) | 19.23 |
| Volatility Index (σ/μ) | **1,530%** |
| Max single win | 150,058 credits |

High volatility profile — typical and expected for a dual progressive jackpot design.

---

## 🎮 Playable Demo

The project includes a fully playable HTML5 demo:

- **No installation required** — open directly in any modern browser
- Animated reels with win line visualization
- Dynamic paytable (updates in real-time with bet changes)
- Synthesized Web Audio sound hierarchy:
  - Subtle eerie sounds for spooky symbol matches
  - Progressive melody for 5-of-5 line wins (~30 seconds)
  - Triumphant melody for Blue Jackpot (~1.5 minutes)
  - Full orchestral theme for Grand Jackpot (~3.5 minutes)
- Auto-spin with melody stop on new spin
- Bet per line: 1–1,000 credits

---

## 🛠️ Technical Stack

| Component | Technology |
|-----------|------------|
| Mathematical model | Python 3 |
| Statistical analysis | `scipy`, `numpy`, `matplotlib` |
| Bayesian inference | `scipy.stats.beta` |
| Simulation | Monte Carlo (10M iterations) |
| Frontend demo | Vanilla HTML5 / CSS3 / Web Audio API |

---

## 📁 Project Structure
dark-fortune-dual-jackpot/
│
├── README.md # This file
├── dark_fortune_2_jackpots.ipynb # Full Python model
├── DEMO_dark_fortune_dual_jackpot.html # Playable HTML5 demo
└── Software_Design_Document.ipynb # Full SDD


---

## 👤 Author

**Dinko Trendafilov**
- GitHub: [DinkoTrendafilov](https://github.com/DinkoTrendafilov)

---

*This project is a mathematical and technical demonstration. No real money is involved.*
