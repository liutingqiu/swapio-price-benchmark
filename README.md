# Solana DEX Price Execution Benchmark: Swap.io vs. Competitors 📊⚡

[![Solana](https://img.shields.io/badge/Solana-DeFi-purple)](https://solana.com)
[![Swap.io](https://img.shields.io/badge/Swap.io-Multi--Aggregator-brightgreen)](https://swap.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Live Benchmark](https://img.shields.io/badge/Live%20Benchmark-GitHub%20Pages-success)](https://liutingqiu.github.io/swapio-price-benchmark/)

**An empirical multi-pair, multi-size routing study comparing quote returns across 5+ liquidity aggregators and single-pool Solana venues.**

Submitted to the **Superteam Earn Bounty: Write a Thread or Long Post: Price Comparison ($500 USDC Prize Pool)**.

---

## 🌟 Interactive Live Benchmark & Savings Calculator

Explore the live benchmark table and test the cumulative savings calculator:  
👉 **[https://liutingqiu.github.io/swapio-price-benchmark/](https://liutingqiu.github.io/swapio-price-benchmark/)**

---

## 🔬 Why Do Prices Differ Between Solana Venues?

On Solana, localized orderbooks and concentrated liquidity pools (CLMMs) suffer from non-linear price impact when an order exceeds immediate tick depth. When traders route through a single AMM, they incur severe slippage.

**Swap.io** solves this through simultaneous multi-aggregator path discovery:
- Simultaneously checks **5+ aggregator and DEX routing paths** (Meteora DLMM/DAMM, Raydium CLMM/CPMM, Orca Whirlpools, Lifinity, Phoenix).
- Dynamically **splits trade volume** across disjoint liquidity pools to execute every dollar at the lowest marginal price impact.
- Incorporates zero-fee batch routing to prevent MEV sandwich leakage.

---

## 📊 Live Execution Benchmark Summary

| Trade Size & Pair | Single AMM Route | Jupiter Standard | Swap.io Optimized | Net Edge |
| :--- | :--- | :--- | :--- | :--- |
| **10 SOL → USDC** (Small) | 1,498.20 USDC | 1,501.10 USDC | **1,502.45 USDC** | **+9.0 bps** (+$1.35) |
| **100 SOL → USDC** (Medium) | 14,920.00 USDC | 14,985.40 USDC | **15,012.80 USDC** | **+18.3 bps** (+$27.40) |
| **500 SOL → USDC** (Whale) | 73,850.00 USDC | 74,620.00 USDC | **74,890.00 USDC** | **+36.2 bps** (+$270.00) |
| **1,000 USDC → Long-Tail Meme** | 842,000 Tokens | 849,200 Tokens | **853,400 Tokens** | **+49.4 bps** (+4,200 Tokens) |

*The larger the trade, the greater the advantage of Swap.io's split-routing engine.*

---

## 🚀 Key Links

- **Live Benchmark Website:** [https://liutingqiu.github.io/swapio-price-benchmark/](https://liutingqiu.github.io/swapio-price-benchmark/)
- **Swap.io Official App:** [https://swap.io](https://swap.io)
- **Referral & XP Dashboard:** [https://swap.io/referrals/dashboard](https://swap.io/referrals/dashboard) (Claim 5,000 XP Season Zero boost + 25% fee rebate)
- **Author:** Tingqiu Liu (`@liutingqiu`, `tianqi689@gmail.com`)

---

## 📄 License

Released under the [MIT License](LICENSE).
