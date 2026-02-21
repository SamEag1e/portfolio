# OHLCraft

> **Status:** On hold | Idea / early planning  
> **Tech Stack:** Python • Planning for: Pytest • Docstrings • MetaTrader5

---

## Overview

**OHLCraft** is a planned Python project aimed at becoming a **minimal, beginner-friendly framework for building trading bots** - inspired by lessons learned while building [CustomTradeBot](../custom-trade-bot/overview.md).

The goal was to simplify the architecture of algo bots by focusing on:

- **Separation of concerns**
- **Modular strategy components**
- **Clear documentation and testability**

---

## Why Build This?

There are already mature trading bot frameworks out there - but most of them:

- Have steep learning curves
- Are designed for advanced use cases or large teams
- Mix too much logic in too few files (or too many abstractions with too little clarity)

OHLCraft is my attempt to create something **simple yet extensible**, something I wish existed when I first started.

---

## Core Vision

The project is on hold - the **architecture was intended to be shaped around real-world lessons**, including:

- How to keep strategy logic isolated and testable
- How to switch between backtest and live modes with minimal changes
- How to fail gracefully in production

Most components will be adapted and polished from CustomTradeBot, with improvements like:

- Docstrings and inline documentation
- Unit tests for core modules
- Clean logging and config control

---

## Progress

So far it’s a [README with a roadmap](https://github.com/SamEag1e/OHLCraft) and some notes from CustomTradeBot. Work is paused.

---

## Lessons & Next Steps

- Not every repo needs to be “done” to be valuable - this one was intended as a **learning playground with potential**
- Planned next steps (when resumed):
  - Modularize CustomTradeBot logic into standalone components
  - Add documentation and tests
  - Explore a plug-and-play config layer for future users

---

## Interested?

If you’re into algo trading, beginner-friendly frameworks, or just want to watch this grow - feel free to **follow**, **fork**, or shoot me ideas.

### 🔙 [Back to Project Index](../README.md)
