# CandleDetect 🔥

CandleDetect is a multi-symbol Smart Money Concepts (SMC) trading bot powered by FastAPI. It supports volatility assets, automated signals, and full API control.

## Features
- Multi-symbol SMC strategy (CHoCH, Order Blocks, FVG)
- Volatility index support (e.g., VIX75, BTCUSD)
- REST API for bot control and signal access
- Docker-ready for cloud deployment
- Automated testing with Pytest

## API Endpoints
- `GET /` – Welcome message
- `GET /status` – Bot status and config
- `POST /start` – Start bot
- `POST /stop` – Stop bot
- `POST /config` – Update bot settings
- `GET /signal?symbol=BTCUSD` – Get trading signal

## Setup
```bash
git clone https://github.com/yourusername/CandleDetect.git
cd CandleDetect
docker build -t candle-detect .
docker run -dp 8000:8000 candle-detect
