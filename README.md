📊 Trader Behavior Analysis Under Bitcoin Market Sentiment (Fear vs Greed)

👤 Author
Anam Alam
📧 anam.alam@lpu.in

🎯Trader Behavior Insights

📌 Introduction
Cryptocurrency markets are highly sentiment-driven, where trader behavior often changes significantly under varying market emotions such as Fear and Greed. Understanding how these sentiment regimes influence trader performance and risk-taking behavior is crucial for designing smarter, data-driven trading strategies.

This project analyzes the relationship between Bitcoin market sentiment and trader performance using real historical trading data and the Bitcoin Fear & Greed Index.

🎯 Project Objective
The primary objectives of this analysis are:

To explore how trader profitability differs between Fear and Greed market regimes

To analyze win rate, risk-taking, and position sizing behavior under different sentiments

To uncover behavioral patterns at both aggregate and trader-specific levels

To statistically validate whether observed differences are significant

The goal is to derive actionable insights that can support smarter trading and risk management decisions.

📂 Datasets Used

1️⃣ Bitcoin Fear & Greed Index
Daily market sentiment classification:

Fear

Extreme Fear

Greed

Extreme Greed

Used to label market regimes on a daily basis

2️⃣ Historical Trader Data (Hyperliquid)
Trade-level data including:

Account

Symbol

Execution price

Position size (USD)

Side (Buy/Sell)

Timestamp

Closed PnL

Leverage

🧠 Methodology & Analysis Workflow
The analysis follows a structured data science pipeline:

Data Cleaning & Preprocessing

Timestamp conversion and date alignment

Handling missing values

Standardizing sentiment categories

Data Integration

Merging daily sentiment data with trader activity

Creating sentiment-aware trade records

Exploratory Data Analysis (EDA)

Performance comparison (Fear vs Greed)

Win rate analysis

Risk and position size analysis

Behavioral Analysis

Risk bucket segmentation

Trader-level performance consistency

Risk vs reward dynamics

Statistical Validation

Mann–Whitney U Test to confirm statistical significance

Validation of performance differences between regimes

Visualization & Storytelling

Clear, insight-driven Python visualizations

Distribution, trend, and relationship analysis

📊 Key Visual Analyses
The notebook includes the following core visualizations:

Average PnL by Market Sentiment

Win Rate Comparison (Fear vs Greed)

PnL Distribution (Boxplot)

Risk vs Reward (Position Size vs PnL Scatter)

Average PnL by Risk Buckets and Sentiment

Correlation Analysis (Optional advanced insight)

Each visualization is accompanied by clear written insights explaining the observed patterns.

🔍 Statistical Validation
A Mann–Whitney U Test was used due to the non-normal, heavy-tailed distribution of PnL

Results show that performance differences between Fear and Greed regimes are statistically significant (p ≪ 0.05)

This confirms that observed behavioral differences are not due to random chance

📈 Key Insights & Findings
Traders generate significantly higher average PnL during Greed periods

Win rates are consistently higher in Greed regimes

Risk-taking is rewarded during Greed but penalized during Fear

PnL distributions are highly skewed, with profits driven by a small number of large wins

Trader performance is regime-dependent, not uniform across market conditions

🛠️ Tech Stack & Tools
Programming Language: Python

Libraries:

pandas

numpy

matplotlib

seaborn

scipy

Environment: Jupyter Notebook

Version Control: Git & GitHub

⚙️ Installation & Setup
Prerequisites
Python 3.8+

Git

Clone the Repository
git clone https://github.com/the-anam/Trader-Behavior-Insights.git
cd Trader-Behavior-Insights
Install Dependencies
pip install -r requirements.txt
▶️ Usage
Open the Jupyter Notebook:

jupyter notebook analysis.ipynb
Run all cells from top to bottom to reproduce:

Data preprocessing

Analysis

Visualizations

Statistical tests

Review:

analysis.ipynb → Full analysis & plots

report.pdf → Detailed written report

presentation.pdf → Executive summary slides

📁 Repository Structure
Trader-Behavior-Insights/
│
├── analysis.ipynb          # Full Python analysis
├── README.md               # Project documentation
├── report.pdf              # Analytical report
├── presentation.pdf        # Summary presentation
├── data/
│   ├── historical_data.csv
│   └── fear_greed_index.csv
└── requirements.txt

🧾 Conclusion
This project demonstrates how market sentiment plays a critical role in shaping trader behavior, profitability, and risk exposure in crypto markets. By combining sentiment analysis with trade-level data and statistical validation, the analysis highlights the importance of sentiment-aware trading strategies.

The workflow reflects an end-to-end data science approach, from raw data to actionable insights, aligned with real-world trading intelligence use cases.

🚀 Future Work
Build predictive models using sentiment as a feature

Cluster traders based on behavioral patterns

Extend analysis to intraday sentiment signals

Apply risk-adjusted performance metrics

📬 Contact
For any questions or feedback:

Anam Alam
📧 anam.alam@lpu.in
