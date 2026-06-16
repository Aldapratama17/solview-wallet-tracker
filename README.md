# solana-airdrop-tracker

> Track all token airdrops received by any Solana wallet. See claim status, token values, and never miss an airdrop again.

![Solana](https://img.shields.io/badge/Solana-mainnet-9945FF?logo=solana&logoColor=white)
![Status](https://img.shields.io/badge/status-live-brightgreen)
![Built with](https://img.shields.io/badge/built%20with-pure%20HTML%2FJS-orange)
![Grant](https://img.shields.io/badge/Superteam-Agentic%20Engineering%20Grant-blue)

## What this is

A dedicated airdrop tracker for Solana wallets. Paste any address and see a full history of received token airdrops — with current value, claim status, and source project.

Solana has distributed billions in airdrops. Most users have no clean way to see what they've received across their wallets. This solves that.

**Live demo:** https://sol-view.netlify.app/

## Features

- Detect airdrop transactions from wallet history
- Classify by token + source protocol
- Current USD value via Jupiter Price API
- Claim status (claimed / unclaimed / expired)
- CSV export for tax / record keeping
- Works for any public Solana address

## Stack

- Pure HTML + Vanilla JS
- Helius RPC for transaction history
- Jupiter Price API for token prices
- Built and tested on Android via Termux

## Project structure

```
solana-airdrop-tracker/
├── index.html          # App shell
├── app.js              # Wallet fetch + airdrop detection logic
├── classifier.js       # Transaction classification engine
├── pricing.js          # Jupiter price integration
├── export.js           # CSV export
├── styles.css          # UI styles
└── README.md
```

## Getting started

```bash
git clone https://github.com/Aldapratama17/solana-airdrop-tracker
cd solana-airdrop-tracker
npx serve .
```

Paste any Solana wallet address. No wallet connection needed.

## How airdrop detection works

1. Fetch last N transactions for the wallet
2. Filter for token transfers where sender ≠ wallet owner
3. Cross-reference against known airdrop distributor programs
4. Classify as airdrop vs. trade vs. transfer
5. Enrich with current price data

## Built by

[@aldapratama47](https://twitter.com/aldapratama47) — solo builder, Solana ecosystem, 5 years.  
Founder of [Onchainhunt](https://github.com/Aldapratama17/onchainhunt-core) · CMO at [Union Build](https://union.build)
