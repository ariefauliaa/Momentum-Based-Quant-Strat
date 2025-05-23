# 📦 Momentum Based Quantitative Strategy

This project looks into an event driven investing strategy that focuses on sectors within the **Jakarta Composite Index (JCI)**, categorized by **Bloomberg GICS industry classification**.

---

### 🧠 Strategy Concept

The core idea is to model how an asset might react to real world sector specific events (supply chain disruptions, geopolitical tensions, and so on) by taking broad exposure to relevant sectors **after** they’ve already shown signs of strength.

Rather than relying on news directly, this strategy identifies sectors that have demonstrated **recent strong momentum**, then enters positions across all stocks within that sector. The logic is reactive, not predictive in order to avoiding forward looking bias.

---

### 🔧 Setup
- **Market**: Jakarta Composite Index (JCI)  
- **Sector Classification**: Bloomberg GICS  
- **Tools**: Python / Jupyter Notebook  
- **Data Logic**: Sector performance filters → basket level exposure
- **Data Source**: Bloomberg Finance LP, Arief Aulia Rakhman  

---

### 📊 Backtest Results

![Backtest Preview](Backtest%20-%20Preview.png)

**Results** 
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

**Fee Assumptions:**  

The above result assumes the use of fee rebates. Without rebates and using the average fee from prop firms (0.01% per tx), the strategy yields a final return of approximately 40,408%.

---

### 🔮 Stress Test - Monte Carlo Simulation

![Monte Carlo Preview](Monte%20Carlo%20-%20Preview.png)

We also ran a **Monte Carlo simulation** to forecast performance over the **next 3 years or 156 weeks**, which supports the strategy’s reliability.

**Parameters**  
| Parameter                     | Value        |
|------------------------------|--------------|
| Historical mean weekly return | 0.5529%      |
| Historical weekly volatility  | 3.7410%      |
| Simulation periods            | 3 years |
| Number of simulations         | 500          |

**Results**  
| Metric                      | Value        |
|----------------------------|--------------|
| Mean final cumulative return | 124.77%     |
| Median final cumulative return | 104.88%   |
| Top 5% outcome              | 303.24%      |
| Bottom 5% outcome           | 0.20%        |
| Probability of positive return | 95.4%     |

**Monte Carlo Interpretation:**  

Using Monte Carlo simulation, the results are impressively strong. When we simulate forward over 3 years, there's a **95.4% chance of ending with a positive return**.

To put that into perspective:  

- Imagine you're blindfolded, and in front of you are **100 toys** some **red** (success) and some **blue** (failure). You reach out and randomly pick **one toy at a time**, doing this **100 times**. Now imagine that **95 of those 100 toys turn out to be red**. That’s how good this strategy’s odds look.
- You **roll a six sided dice 100 times and land on a six 95 times**. That’s not random anymore, that’s a strategy on steroids.

And it’s not just about *not losing*. The **mean return** of **124.77% over 3 years** equates to CAGR of roughly **30.5%**, which is **excellent** especially considering the conservative, reactionary nature of the strategy.

---

### 🎯 Objective

To evaluate whether **reactive sector exposure** can yield positive returns when applied systematically and without hindsight.

---

📁 **Note:**  
The Jupyter notebook containing the full backtest is **private**.  
Feel free to reach out via email for access.  
📧 [ariefauliaa@gmail.com]
