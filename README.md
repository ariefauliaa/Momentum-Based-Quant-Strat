# 📦 Momentum-Based Strategy

This repository explores a sector-based event investing approach using stocks from the **Jakarta Composite Index (JCI)**, categorized by **Bloomberg GICS industry classification**.

---

### 🧠 Strategy Concept

The core idea is to simulate how an investor might respond to real-world sector-specific events (e.g., supply chain disruptions, geopolitical tensions) by taking broad exposure to relevant sectors **after** they’ve already shown signs of strength.

Rather than relying on news directly, this strategy identifies sectors that have demonstrated **recent strong momentum**, then enters positions across all stocks within that sector. The logic is reactive, not predictive — avoiding forward-looking bias.

---

### 🔧 Setup
- **Market**: Jakarta Composite Index (JCI)  
- **Sector Classification**: Bloomberg GICS  
- **Tools**: Python / Jupyter Notebook  
- **Data Logic**: Sector performance filters → basket-level exposure
- **Data Source**: Bloomberg Finance LP, Arief Aulia Rakhman  

---

### 📊 Backtest Results

![Backtest Preview](Backtest%20Preview%20-%20Momentum%20Based.png)

| Metric                    | Value            |
|---------------------------|------------------|
| **Period**                | 2000-10-22 to 2025-04-13 |
| **Initial Balance**       | Rp1,000,000       |
| **Final Balance**         | Rp432,246,719     |
| **Total Return**          | 42,588.93%        |
| **Annualized Return**     | 28.08%            |
| **Annualized Volatility** | 28.45%            |
| **Sharpe Ratio**          | 0.99              |
| **Max Drawdown**          | -56.18%           |
|                           |                  |
| **Benchmark Return**      | 1,939.33%         |
| **Benchmark Max Drawdown**| -59.50%           |
| **Total Alpha**           | 40,649.60%        |
| **Annualized Alpha**      | 27.84%            |

📌 Fee Assumptions:
- Uses a transaction fee of **0.01% per trade**, a typical average in **prop trading firms**.
- If **fee rebates** are applied (HFT environments), the strategy could reach a **final return of up to 48,400%**, showing significantly enhanced profitability under more favorable cost structures.

---

### 🎯 Objective

To evaluate whether **reactive sector exposure** — mimicking event-driven investing — can yield positive returns when applied systematically and without hindsight.

---

📁 **Note:**  
The Jupyter notebook containing the full backtest is **private**.  
Feel free to reach out via email for access.  
📧 [ariefauliaa@gmail.com]
