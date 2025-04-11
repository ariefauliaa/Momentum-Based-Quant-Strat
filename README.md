# 📦 Sector Event-Based Backtest (JCI + GICS)

This repository explores a sector-based event investing approach using stocks from the **Indonesia Stock Exchange (JCI)**, categorized by **Bloomberg GICS industry classification**.

---

### 🧠 Strategy Concept

The core idea is to simulate how an investor might respond to real-world sector-specific events (e.g., supply chain disruptions, geopolitical tensions) by taking broad exposure to relevant sectors **after** they’ve already shown signs of strength.

Rather than relying on news directly, this strategy identifies sectors that have demonstrated **recent strong momentum**, then enters positions across all stocks within that sector. The logic is reactive, not predictive — avoiding forward-looking bias.

---

### 🔧 Setup
- **Market**: Indonesia Stock Exchange (JCI)  
- **Sector Classification**: Bloomberg GICS  
- **Tools**: Python / Jupyter Notebook  
- **Data Logic**: Sector performance filters → basket-level exposure  

---

### 📊 Backtest Results

| Metric                    | Value            |
|---------------------------|------------------|
| **Period**                | 2000-10-22 to 2025-04-13 |
| **Initial Balance**       | Rp1,000,000       |
| **Final Balance**         | Rp913,281,339     |
| **Total Return**          | 90,087.27%        |
| **Annualized Return**     | 32.05%            |
| **Annualized Volatility** | 30.54%            |
| **Sharpe Ratio**          | 1.05              |
| **Max Drawdown**          | -61.88%           |
|                           |                  |
| **Benchmark Return**      | 1,939.33%         |
| **Benchmark Max Drawdown**| -59.50%           |
| **Total Alpha**           | 88,147.94%        |
| **Annualized Alpha**      | 31.94%            |

---

### 🎯 Objective

To evaluate whether **reactive sector exposure** — mimicking event-driven investing — can yield positive returns when applied systematically and without hindsight.

---

📁 **Note:**  
The Jupyter notebook containing the full backtest is **private**.  
If you're a **recruiter or headhunter**, feel free to reach out via email for access.  
📧 [your.email@example.com]