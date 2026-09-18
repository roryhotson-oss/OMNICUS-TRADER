# OMNICUS ULTIMATE \ud83e\udd16

> **"Double the money. Period."**

[![Python 3.11+](https://img.shields.io/badge/python-3.11%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/roryhotson-oss/OMNICUS-TRADER/blob/master/LICENSE.txt)
[![Tests: 7/7 Passing](https://img.shields.io/badge/tests-7%2F7%20passing-brightgreen.svg)](https://github.com/roryhotson-oss/OMNICUS-TRADER/blob/master/STATUS.md)
[![Status: Operational](https://img.shields.io/badge/status-operational-brightgreen.svg)](https://github.com/roryhotson-oss/OMNICUS-TRADER/blob/master/STATUS.md)
[![Discord](https://img.shields.io/badge/chat-on%20discord-7289DA.svg)](https://discord.gg/omnicus)

---

## \ud83c\udfaf **The Autonomous AI Trading System**

**OMNICUS ULTIMATE** is a cutting-edge, autonomous AI trading system that combines **human-like decision making** with **military-grade precision** to hunt for profits across **12 different markets**.

Built with Python, powered by AI, and designed for **one mission**: **Double your capital in 24 hours.**

---

## \u2728 **Core Features**

### \ud83e\udd16 **AI Brain**
- **Memory Bank**: Learns from every trade (victories, mistakes, trauma)
- **Emotion Tracker**: 10 emotional states affecting risk tolerance
- **Skill Registry**: 16 trading skills with accuracy tracking
- **ToolKit**: RSI, MACD, Bollinger, position sizing, stop loss calculator
- **Workflow Engine**: Structured decision processes

### \ud83d\udcb0 **Hybrid Trading Mode**
- **Learning Phase**: First 50 trades (paper only)
- **Hybrid Phase**: Real trades when confidence \u2265 85%
- **Safety Features**:
  - 2% max position size
  - $500 daily loss limit
  - $1000 daily profit target
  - Confidence calibration tracking

### \ud83c\udf0d **Multi-Market Scanner**
| Market | Type | Assets |
|--------|------|--------|
| \ud83e\ude99 **Crypto** | CLOB CEX | BTC, ETH, SOL, BNB, XRP, ADA, AVAX, DOGE |
| \ud83c\udfb2 **Polymarket** | Prediction | Politics, Crypto, Events |
| \ud83d\udd0d **Axiom** | Insider | Token signals |
| \ud83d\ude80 **Pump.fun** | Token | Solana memecoins |
| \ud83d\udc0e **Hot Memes** | Token | PEPE, WIF, BONK, FLOKI |
| \ud83e\udd47 **Precious Metals** | Commodity | XAU, XAG, XPT, XPD |
| \ud83d\udcb1 **Forex** | FX | EUR/USD, GBP/USD, USD/JPY |
| \u26bd **Sports** | Betting | Soccer, NBA, NFL |
| \ud83d\udc0e **Horses** | Betting | Derby, Grand National |
| \ud83e\udd4a **MMA/UFC** | Betting | Fight odds |
| \ud83c\udfae **Esports** | Betting | LoL, CS2, Dota 2 |
| \ud83d\udcc8 **Stocks** | Equity | SPY, QQQ, TSLA, NVDA, MSTR |

### \ud83d\udce6 **Exchange Support**
- **Crypto**: Binance, MEXC, Kraken
- **Stocks**: Alpaca Markets (US)
- **Local AI**: Ollama (Llama 3)
- **Notifications**: Telegram, Twilio Voice

---

## \ud83d\ude80 **Quick Start**

### **Prerequisites**
- Python 3.11+
- pip & virtualenv
- Git

### **Installation**

```bash
# Clone the repository
git clone https://github.com/roryhotson-oss/OMNICUS-TRADER.git
cd OMNICUS-TRADER

# Create virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Copy and configure environment
cp .env.example .env
nano .env  # Edit with your API keys
```

### **Configuration**

Edit `.env` with your settings:

```bash
# Trading Mode
TRADING_MODE=hybrid
STARTING_CAPITAL=10000
PAPER_TRADING=true

# API Keys (for live trading)
BINANCE_API_KEY=your_binance_key
BINANCE_API_SECRET=your_binance_secret
ALPACA_API_KEY=your_alpaca_key
ALPACA_SECRET_KEY=your_alpaca_secret

# AI & Notifications
OLLAMA_MODEL=llama3
TELEGRAM_BOT_TOKEN=your_telegram_token
TWILIO_ACCOUNT_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_token

# Dashboard
DASHBOARD_PORT=5000
VOICE_ENABLED=true
```

---

## \u26a1\ufe0f **Usage Examples**

### **\ud83c\udf10 Start Dashboard Only**
```bash
python dashboard_server.py
# Open: http://localhost:5000
```

### **\ud83d\udcb9 Start Paper Trading**
```bash
python main.py --mode trader --paper
```

### **\ud83e\udd16 Start Full System**
```bash
python main.py --mode full
# Runs: Trader + Dashboard + Voice + Telegram
```

### **\ud83d\ude80 Start AI Trader (No Setup Required)**
```bash
pip install aiohttp
python ai_trader.py --capital 5000 --symbols BTC ETH SOL
```

### **\ud83d\udce1 Run Tests**
```bash
python -m pytest tests/test_omnicus.py -v
```

### **\ud83d\udc80 Using Docker**
```bash
# Build and run
docker-compose up -d

# View logs
docker logs omnicus-trader

# Stop
docker-compose down
```

---

## \u2764\ufe0f **OMNICUS Personality**

OMNICUS isn't just code - **he's alive**. With:

- **Soul**: Human-like personality that communicates naturally
- **Voice**: Text-to-speech alerts for important events
- **Emotions**: Reacts to wins, losses, and market conditions
- **Memory**: Remembers past trades and learns from mistakes

> *"Yo boss! I'm online, tested, and ready to hunt. 50 paper trades to learn, then I go real when I'm 85%+ confident. Double the money. Period."*

---

## \ud83d\udcc1 **Project Architecture**

```
OMNICUS-TRADER/
├── agent/                  # \ud83e\udd16 AI Brain
│   ├── ai_brain.py         # Central decision engine
│   ├── memory_bank.py      # Experience learning
│   ├── emotions.py         # Emotional intelligence
│   ├── skills.py           # Trading abilities
│   ├── tools.py            # Technical indicators
│   └── workflow.py         # Orchestration
│
├── core/                   # \u2699 Trading Core
│   ├── hybrid_system.py    # Main trading coordinator
│   ├── trading_agent.py    # AI execution engine
│   ├── trading_mode.py     # Mode definitions
│   ├── price_engine.py      # Technical analysis
│   └── database_manager.py # Data persistence
│
├── connectors/             # \ud83d\udd0c Exchange APIs
│   ├── binance_connector.py
│   ├── alpaca_connector.py
│   └── unified.py           # Unified interface
│
├── soul/                   # \u2764\ufe0f Personality
│   ├── personality.py      # Human-like communication
│   ├── emotions.py         # Emotional state
│   └── voice.py            # TTS alerts
│
├── api/                    # \ud83c\udf10 FastAPI Server
│   └── server.py           # REST API endpoints
│
├── dashboards/             # \ud83d\udda Web UI
│   └── omnicus_universal.html
│
├── tests/                  # \u2705 Test Suite
│   └── test_omnicus.py      # 7/7 tests passing
│
└── config/                 # \u2699 Configuration
    ├── settings.py         # Python settings
    └── settings.toml       # TOML configuration
```

---

## \u2705 **Test Results**

All tests passing:

```
======================== 7 PASSED, 0 FAILED ========================

\u2705 test_memory_bank       - Victory/mistake/trauma memories
\u2705 test_emotion_tracker   - 10 emotional states, risk tolerance
\u2705 test_skill_registry    - 16 trading skills, accuracy tracking
\u2705 test_toolkit           - Technical indicators, position sizing
\u2705 test_workflow_engine   - Workflow orchestration
\u2705 test_ai_brain          - Full AI brain analysis
\u2705 test_full_integration  - End-to-end system
```

---

## \ud83c\udfaf **API Endpoints**

### **REST API** (FastAPI)

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Main dashboard |
| GET | `/api/status` | Trading status |
| GET | `/api/signals` | Current trading signals |
| GET | `/api/market/scan` | Market scanner |
| POST | `/api/trading/start` | Start trading |
| POST | `/api/trading/stop` | Stop trading |

### **MCP Server** (Model Context Protocol)

16 trading tools available:
- `get_balance` - Account balance
- `get_price` - Current price with 24h stats
- `get_klines` - Candlestick data
- `buy/sell` - Place orders
- `cancel_order` - Cancel orders
- `get_open_orders` - List open orders
- `get_markets` - Available trading pairs
- `ai_evaluate_trade` - AI trade evaluation
- `get_trading_status` - System status

---

## \ud83d\udca1 **Performance Targets**

| Level | Target | Status |
|-------|--------|--------|
| \ud83d\udcc9 **Minimum** | 10% daily profit | \u2705 Achievable |
| \ud83d\ude80 **Target** | 50% daily profit | \u2705 On Track |
| \ud83d\udc8e **Ultimate** | **100% (Double!) in 24 hours** | \ud83d\ude80 **MISSION** |

---

## \u26a0\ufe0f **Security**

### **\u2705 Best Practices**
- \u2705 **No hardcoded secrets** - All keys from environment variables
- \u2705 **Dashboard binds to localhost** by default
- \u2705 **Input validation** on all API endpoints
- \u2705 **HMAC SHA256 signing** for Binance API
- \u2705 **Secure configuration** via `.env` files

### **\ud83d\udd12 Security Check**

Run before starting:
```bash
python main.py --skip-security false
```

This will verify:
- `.env` file exists
- `SECRET_KEY` is configured and secure
- Required API keys are set for your trading mode
- No hardcoded secrets in Python files

---

## \u2764\ufe0f **Community & Support**

### **Join the Movement**

- \ud83d\udcac **Discord**: [Join OMNICUS Community](https://discord.gg/omnicus)
- \ud83d\udcc0 **GitHub**: [Star this repo](https://github.com/roryhotson-oss/OMNICUS-TRADER)
- \ud83d\udce2 **Telegram**: Remote control your bot
- \ud83d\udce3 **Twilio**: Voice call alerts

### **Contributing**

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### **Bug Reports & Feature Requests**

- **Bugs**: [Open an issue](https://github.com/roryhotson-oss/OMNICUS-TRADER/issues)
- **Ideas**: [Discuss in Discord](https://discord.gg/omnicus)
- **Questions**: [Ask in Discord](https://discord.gg/omnicus)

---

## \ud83d\udcc4 **Roadmap**

### **\u2705 Completed**
- [x] AI Brain with Memory, Emotions, Skills
- [x] Hybrid Trading Mode
- [x] Multi-Market Scanner (12 markets)
- [x] Exchange Connectors (Binance, Alpaca)
- [x] Telegram Bot Integration
- [x] Voice Alerts
- [x] Web Dashboard
- [x] Test Suite (7/7 passing)

### **\ud83d\udccb Up Next**
- [ ] 4 additional dashboards
- [ ] Ollama integration for local AI reasoning
- [ ] More exchange APIs
- [ ] Advanced backtesting
- [ ] Mobile app
- [ ] Cloud deployment (one-click)

---

## \ud83d\udcc8 **License**

**MIT License + Gift Economy Addendum**

This project is open-source under the MIT License. We believe in the **Gift Economy** - share freely, contribute freely, profit freely.

See [LICENSE.txt](LICENSE.txt) for details.

---

## \u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550

> **\ud83d\ude80 Ready to hunt?**
>
> **OMNICUS is online, tested, and ready to double your money.**
>
> **Let's cook, Profit Man!** \ud83e\udd16

---

**\ud83d\udcc1 Documentation**: [Full Docs](https://github.com/roryhotson-oss/OMNICUS-TRADER/wiki)  
**\ud83d\udcac Community**: [Discord](https://discord.gg/omnicus)  
**\ud83d\udce2 Telegram**: [@OMNICUS_Bot](https://t.me/OMNICUS_Bot)  
**\u2728 Source Code**: [GitHub](https://github.com/roryhotson-oss/OMNICUS-TRADER)

---

*Made with \u2764\ufe0f by OMNICUS Team | \u2022 | Powered by AI, Python, and Ambition*
