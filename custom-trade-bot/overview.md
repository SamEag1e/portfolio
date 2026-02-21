# Custom Trade Bot

> **Status:** Not actively developed | Private Codebase | Notification mode in use  
> **Tech Stack:** Python • MetaTrader5 • Plotly

---

## Overview

Custom Trade Bot is a Python-based trading bot I built for **both live trading and backtesting** with full **MetaTrader5 integration**.

It was built around a custom trading strategy and includes **modular components** for signal generation, dynamic order handling, and bot control.

The codebase is private; screenshots are provided and a walkthrough can be provided on request.

---

## Key Features

### MetaTrader5 Integration

- Connects to **MetaTrader5** for real-time market data, order placement, and account tracking.
- Efficient handling of broker interactions and API edge cases.

### Strategy & Logic

- Executes trades based on **client-defined entry conditions** and signals
- Supports **custom structures** like:
  - Fair Value Gaps (FVG)
  - Liquidity
  - Trend
  - Multi-factor entry signals

### Custom Order Handling

- Flexible logic to generate **market and limit orders**
- Dynamic control over:
  - **Lot sizing**
  - **Stop-loss / Take-profit**
  - Conditional re-entry and risk settings

### Dual Modes: Live + Backtest

- Backtest strategies on historical data with consistent execution logic
- Seamless switch to **live mode** using the same config and entry logic

### Real-Time Control System

- Behavior is controlled by a `status.txt` file for:
  - Emergency shutdowns (`kill all`)
  - Enabling/disabling trading without restarting
  - Fine-tuned debug and verbosity levels

### Logging & Visualization

- Real-time logging of decisions and trades
- Performance analytics and **backtest visualizations** using **Plotly**

### Status & Refactor Notes

- Live trading was disabled; the bot runs in **notification-only mode**
- The codebase was **refactored for better modularity and separation of concerns**
- Screenshots of Telegram alerts and the improved code structure are included

---

## Screenshots

![trade-bot-backtest-plotly](./assets/trade-bot-backtest-plotly-fig.png)
![trade-bot-results-log](./assets/trade-bot-results-log.png)
![trade-bot-refactor](./assets/trade-bot-refactor.png)
![trade-bot-working-terminal](./assets/trade-bot-working-terminal.png)
![trade-bot-notifications](./assets/trade-bot-notifications.png)

---

## Access or Demo

<p>
    <a href="mailto:samadeagle@yahoo.com" target="_blank" rel="noreferrer">
    <img src="https://img.icons8.com/fluency/20/new-post.png" width="20" height="20" alt="Email" style="display:inline; margin: 0 6px;" />
    </a>
    <a href="https://wa.me/989146446078" target="_blank" rel="noreferrer">
    <img src="https://img.icons8.com/color/20/whatsapp--v1.png" width="20" height="20" alt="WhatsApp" style="display:inline; margin: 0 6px;" />
    </a>
    <a href="https://t.me/SamadTnd" target="_blank" rel="noreferrer">
    <img src="https://img.icons8.com/ios-filled/20/0088cc/telegram-app.png" width="20" height="20" alt="Telegram" style="display:inline; margin: 0 6px;" />
    </a>
    <a href="https://www.linkedin.com/in/samad-taghinejad/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin.svg" width="20" height="20" alt="LinkedIn" style="display:inline; margin: 0 6px;" />
    </a>
</p>
I’m open to collaborations, freelance opportunities, or contributions under NDA.

---

## Lessons & Next Steps

- Delivered a working bot that met all client requirements for live trading on a demo account
- Learned how to build a fault-tolerant system for **real-world trading**, including exception handling, session control, and real-time monitoring
- The bot is used as a **signal-notification system**: multiple instances ran on different Forex pairs, pushing alerts to a Telegram group when predefined "scenarios" were met; the client applied additional filters manually before executing trades

### Related Project: [OHLCraft](https://github.com/SamEag1e/OHLCraft)

> This project inspired the creation of **OHLCraft**, a WIP open-source framework for building modular trading bots.  
> [View the OHLCraft showcase](../ohlcraft/overview.md)

### 🔙 [Back to Project Index](../README.md)
