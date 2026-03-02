Binance Futures Testnet Trading Bot
📌 Overview

This project is a modular, CLI-based trading application built in Python that interacts with the Binance Futures Testnet (USDT-M).

It enables users to place Market, Limit, and Stop-Limit orders with proper input validation, structured logging, and robust error handling.

The project emphasizes clean architecture, separation of concerns, and production-level reliability practices.

🚀 Features

✅ Supports BUY and SELL sides

✅ Order types:

MARKET

LIMIT

STOP_LIMIT (Stop-Limit)

✅ Command-line interface using argparse

✅ Input validation before API execution

✅ Structured logging of API requests and responses

✅ Exception handling for API and runtime errors

✅ Modular and reusable code architecture

🏗 Project Structure
binance-futures-trading-bot/
│
├── bot/
│   ├── client.py          # Binance client wrapper
│   ├── orders.py          # Order execution logic
│   ├── validators.py      # Input validation
│   ├── logging_config.py  # Logging configuration
│
├── cli.py                 # CLI entry point
├── requirements.txt
├── README.md
⚙️ Setup Instructions
1️⃣ Clone the Repository
git clone <your-repository-url>
cd binance-futures-trading-bot
2️⃣ (Optional) Create Virtual Environment
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows
3️⃣ Install Dependencies
pip install -r requirements.txt
4️⃣ Configure Environment Variables

Create a .env file in the project root:

API_KEY=your_api_key
API_SECRET=your_api_secret
▶️ Usage Examples
🔹 Market Order
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001
🔹 Limit Order
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 60000
🔹 Stop-Limit Order
python cli.py --symbol BTCUSDT --side BUY --type STOP_LIMIT --quantity 0.001 --price 59000 --stop-price 59500
📝 Logging

All API interactions, request summaries, responses, and errors are logged in:

trading_bot.log

Logging is implemented to improve traceability, debugging, and reliability.

🔐 Assumptions

Binance Futures Testnet account is active

Valid API credentials are provided

Sufficient testnet balance is available for order execution

📎 Notes

This project was built as part of an internship technical assessment to demonstrate:

Clean code structure

API integration

Input validation

Logging and reliability handling

Practical understanding of trading order types
