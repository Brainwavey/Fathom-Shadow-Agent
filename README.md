# 🛡️ Fathom OS: Shadow Agent
**Private Market Intelligence Pipeline built with SolRouter Encrypted AI.**

### The Problem
In Web3, alpha is everything. If a trader uses a public LLM (like ChatGPT) to analyze token metrics or research new wallets, their strategy is leaked to centralized servers. 

### The Solution
The **Fathom Shadow Agent** is a Python-based data pipeline that routes market analysis prompts through [SolRouter's](https://solrouter.com) encrypted inference network. 

By utilizing the SolRouter SDK (via OpenAI compatible endpoints), prompts are encrypted locally and processed within isolated hardware on Solana. The researcher gets high-level AI analysis without exposing their target tokens or trading strategies.

### Technical Architecture
* **Language:** Python
* **Framework:** SolRouter Encrypted Llama (`solrouter-private-llama`)
* **Integration:** Direct API payload routing via `requests` to bypass SDK strict-schema limitations during Devnet testing.
* **Status:** Pipeline operational. Includes a local mock-inference fallback designed to keep the Fathom OS system running smoothly when the SolRouter Devnet experiences DNS resolution timeouts.
