# Binance Futures Testnet Trading Bot

## Overview
A CLI-based trading bot built in Python that places MARKET and LIMIT orders on Binance Futures Testnet (USDT-M).

## Features
- BUY and SELL orders
- MARKET and LIMIT support
- CLI input validation
- Logging of API requests and responses
- Exception handling

## Setup

1. Clone repository
2. Install dependencies:
   pip install -r requirements.txt
3. Add API keys in .env file
4. Run examples:

Market Order:
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001

Limit Order:
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 60000

## Logs
Logs are stored in trading_bot.log

## Assumptions
- Binance Futures Testnet account active
- Valid API keys provided
