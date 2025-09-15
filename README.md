# **NAITradingBot**

**NAITradingBot - Neural Artificial Intelligence Trading Bot** is an automated cryptocurrency trading agent that connects to the Binance API and executes trades based on a neural network and multiple technical indicators (RSI, MACD, EMA, SMA, breakout/breakdown signals).

The bot has been tested in both Testnet and Mainnet environments and supports real-time execution with live market data through Binance WebSocket streams and logs all trades in CSV format.

---

## 🚀 Features

- ✅ **Binance API Integration** – Works with Binance Testnet & Mainnet.
- ✅ **Automated Trading** – Executes buy/sell orders based on neural network predictions + indicators.
- ✅ **Multi-Indicator Strategy** – RSI, EMA, SMA, MACD, breakout/breakdown logic.
- ✅ **Neural Network Model** – Deep Q-Learning agent with Dense layers.
- ✅ **Trade Logging** – All trades saved in CSV with timestamp, order ID, and fee.
- ✅ **Experience Replay** – Saves and reloads model + past experiences (pickle + TensorFlow checkpoint).

---

🛠️ Installation
Requirements

Python 3.9+

Binance API

Required libraries:

```Python
pip install numpy
pip install pandas
pip install tensorflow
pip install keras
pip install nest-asyncio
pip install requests
```

Stable version libraries:

```Python
pip install python-binance==1.0.19
pip install websockets==12.0
```

⚙️ Configuration

Change your keys in this code part 

# For Testnet
```Python
# Binance Testnet API keys
api_key = "YOUR_TESTNET_KEY"
api_secret = "YOUR_TESTNET_SECRET"
client = Client(api_key, api_secret, testnet=True)
```

Create a new API Key & Secret from Binance API Management.

Enable Spot & Margin Trading.

Do NOT enable withdrawals. 

# For Mainnet
```Python
# Binance Mainnet API keys
api_key = "YOUR_MAINNET_KEY"
api_secret = "YOUR_MAINNET_SECRET"
client = Client(api_key, api_secret)
```

▶️ Usage

Run the bot with:

python main.py


Example trade log:

```
Buy order executed at Price 4395.81 USDT | 0.0022 ETH | Total: 9.67 USDT | 2025-08-12 16:12:38
Sell order executed at Price 4405.34 USDT | 0.0022 ETH | Total: 9.68 USDT | 2025-08-12 16:28:03
```

📊 Example Results (Mainnet Test – ETH/USDT, 12 Aug 2025)

Number of round-trips: 38

Total Profit: +0.230456 USDT

ROI: 0.0621%

Win rate: 63.2%

Best trade: +0.09735 USDT

Worst trade: -0.040876 USDT

🧠 Roadmap

 Add multi-agent reinforcement learning models (PPO, DQN).

 Implement portfolio management (multi-pair trading).

 Deploy on cloud (AWS / GCP / DigitalOcean).

 Dashboard for visualization of live trades.

## ⚠️ Disclaimer

This project is provided for educational and research purposes only.
Trading cryptocurrencies carries a high level of risk and may not be suitable for all investors.
The authors and contributors of this repository do not provide financial advice and are not responsible for any financial losses, damages, or consequences resulting from the use of this software.

Always test on Binance Testnet before using on Mainnet.

Use your own risk management strategies.

Past performance does not guarantee future results.

Use at your own risk.


## Authors

- [@nderimajdari](https://github.com/nderimajdari)

