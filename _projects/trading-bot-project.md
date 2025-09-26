# Project: Binance Mock Trading Bot

A sophisticated, command-line trading bot written in Python that simulates placing complex futures orders on the Binance exchange without requiring real credentials or funds.

[Back to Home](./index.md)

---

### 1. The Goal
The objective was to create a Python-based CLI trading bot to demonstrate a deep understanding of the Binance API, complex order types (Market, Limit, Stop-Limit), and robust software design. The entire system is built to use mock responses, allowing for safe and thorough testing of the bot's logic without any financial risk or need for API keys.

---

### 2. My Role & Contributions
As the sole developer, I architected and built the entire application with a focus on clean code and separation of concerns.

* **Core Bot Logic:** I developed the main engine in `bot.py` to handle the logic for different order types and sides (BUY/SELL), ensuring the correct parameters were used for each.
* **API Simulation:** I created a `mock_binance.py` module to accurately simulate the response structure of the real Binance API. This allowed for isolated testing and development of the bot's interaction logic.
* **User Interface (CLI):** I built an interactive and user-friendly command-line interface in `cli.py` that guides the user through the trading process, implementing strong input validation to prevent errors.
* **Modular Architecture:** I designed the project with a clean, modular structure, separating the CLI, bot logic, and mock API into distinct files for better readability, maintenance, and reusability.

---

### 3. Technologies Used
* **Core Language:** Python
* **Application Type:** Command-Line Interface (CLI) Tool
* **Key Concepts:** API Simulation, Input Validation, Modular Software Design

---

### 4. Project Links
* **[View Code on GitHub](https://github.com/githubabhay2003/binance-mock-trading-bot-assignment)**
