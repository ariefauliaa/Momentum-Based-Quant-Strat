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
| **Final Balance**         | Rp490,888,775     |
| **Total Return**          | 48,375.66%        |
| **Annualized Return**     | 28.75%            |
| **Annualized Volatility** | 26.99%            |
| **Sharpe Ratio**          | 1.06              |
| **Max Drawdown**          | -56.19%           |
|                           |                  |
| **Benchmark Return**      | 1,939.33%         |
| **Benchmark Max Drawdown**| -59.50%           |
| **Total Alpha**           | 46,463.33%        |
| **Annualized Alpha**      | 28.53%            |

Fee Assumptions: The above result assumes the use of fee rebates. Without rebates and using the average fee from prop trading firms (0.01% per trade), the strategy yields a final return of approximately 40,408%.

---

### 🎯 Objective

To evaluate whether **reactive sector exposure** — mimicking event-driven investing — can yield positive returns when applied systematically and without hindsight.

---

📁 **Note:**  
The Jupyter notebook containing the full backtest is **private**.  
Feel free to reach out via email for access.  
📧 [ariefauliaa@gmail.com]
