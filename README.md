# 🚀 PumpFun Trading Bot

An automated trading bot for [pump.fun](https://pump.fun) built on the Solana blockchain. Monitor new token launches, analyze bonding curves, and execute sniper/sell strategies — all from the command line.

🌐 **Live Demo & Landing:** [pump-analyzer.org](https://www.pump-analyzer.org)

---

## ✨ Features

- 🔍 **Real-time token monitoring** — track new token launches on pump.fun via WebSocket
- 📈 **Bonding curve analysis** — evaluate token progress and market cap in real time
- 🎯 **Sniper bot** — automatically buy tokens at launch based on configurable filters
- 💰 **Auto-sell strategies** — set take-profit and stop-loss targets
- 🗂️ **Trade logging** — all trades saved locally for review
- ⚙️ **Fully configurable** — customize slippage, priority fees, filters, and more

---

## 📋 Requirements

- Python 3.11+
- A Solana wallet with SOL for trading
- [Chainstack](https://chainstack.com) RPC endpoint (or any Solana RPC)

---

## ⚡ Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/angelfaceburgh49ez3/pumpfun-trading-bot/git
cd congenial-happiness

# 2. Install dependencies
pip install .

# 3. Configure environment
cp .env.example .env
# Edit .env with your private key and RPC URL

# 4. Run the bot
python -m src.main
```

---

## 🔧 Configuration

Copy `.env.example` to `.env` and fill in your values:

```env
PRIVATE_KEY=your_solana_wallet_private_key
RPC_URL=https://your-chainstack-or-other-rpc-endpoint
WSS_URL=wss://your-chainstack-or-other-wss-endpoint
```

All trading parameters (buy amount, slippage, filters, take-profit, stop-loss) are configurable inside the `src/` modules.

---

## 📁 Project Structure

```
├── bots/           # Bot strategy implementations
├── src/            # Core logic (monitor, sniper, trader)
├── trades/         # Local trade history logs
├── .env.example    # Environment variable template
├── pyproject.toml  # Project dependencies
└── README.md
```

---

## ⚠️ Disclaimer

This bot is provided for **educational purposes only**. Trading meme coins is extremely risky. Never trade with funds you cannot afford to lose. The authors are not responsible for any financial losses.

---

## 📄 License

MIT License
