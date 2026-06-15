# solview-wallet-tracker
Solana wallet portfolio tracker — built with AI coding tools as part of Superteam grant.
solana-airdrop-tracker
Track all token airdrops received by any Solana wallet. See claim status, token values, and never miss an airdrop again.
�
�
�
�
Muat gambar
Muat gambar
Muat gambar
Muat gambar
What this is
A dedicated airdrop tracker for Solana wallets. Paste any address and see a full history of received token airdrops — with current value, claim status, and source project.
Solana has distributed billions in airdrops. Most users have no clean way to see what they've received across their wallets. This solves that.
Live demo: [your-deployed-url-here]
Features
Detect airdrop transactions from wallet history
Classify by token + source protocol
Current USD value via Jupiter Price API
Claim status (claimed / unclaimed / expired)
CSV export for tax / record keeping
Works for any public Solana address
Stack
Pure HTML + Vanilla JS
Helius RPC for transaction history
Jupiter Price API for token prices
Built and tested on Android via Termux
Project structure
Kode
Getting started
Bash
Paste any Solana wallet address. No wallet connection needed.
How airdrop detection works
Fetch last N transactions for the wallet
Filter for token transfers where sender ≠ wallet owner
Cross-reference against known airdrop distributor programs
Classify as airdrop vs. trade vs. transfer
Enrich with current price data
Built by
@aldapratama47 — solo builder, Solana ecosystem, 5 years.
Founder of Onchainhunt · CMO at Union Build
