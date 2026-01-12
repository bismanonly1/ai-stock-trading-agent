# Machine Learning Stock Trading Agent

An educational, bottom-up built AI agent that predicts top-performing stocks, simulates daily trading with hourly monitoring & adjustments, and generates EOD reports — all using Machine Learning (starting simple with RandomForest).

**Goal**: Demonstrate end-to-end ML + Finance skills for learning & job applications (quant dev, data scientist, algo trader roles).

## Project Philosophy
- Bottom-up learning: start from single stock data → indicators → dataset → model → simulation → full agent
- Clean, modular code with good documentation
- Emphasis on understanding, not black-box magic
- Simulation/paper trading only — **not real money trading**

## Current Status (as of Jan 2026)
- [x] Single stock data exploration (yfinance)
- [ ] Technical indicators & feature engineering
- [ ] Dataset creation (multi-stock)
- [ ] First ML model (Random Forest)
- [ ] Portfolio simulation & P/L calculation
- [ ] Hourly monitoring logic
- [ ] Scheduled agent (pre-market / hourly / EOD)
- [ ] Professional reporting & visualization

## Key Learning Areas Covered
- Time-series data handling with pandas & yfinance
- Feature engineering (technical indicators: returns, SMA, RSI, ...)
- Supervised ML for regression/classification in finance
- Backtesting & simulation pitfalls (lookahead bias, survivorship, etc.)
- Modular code architecture
- Automation with scheduling

## How to Run (once complete)

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Run exploratory notebooks (in order)
jupyter notebook notebooks/

# 3. Run the full simulation agent
python src/scheduling/agent.py --mode=simulate --date=2025-12-01