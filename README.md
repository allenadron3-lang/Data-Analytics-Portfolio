# Data Analytics Portfolio

A collection of data analysis projects showcasing skills in data cleaning, exploratory analysis, statistical modeling, and business insight generation using Python.

## 📊 Projects

### 1. E-Commerce Sales Analysis
**File:** `Ecommerce.ipynb`

An analysis of UK-based online retail transaction data (Dec 2010–Dec 2011) to uncover sales trends, customer behavior, and revenue drivers.

**What this project covers:**
- Data cleaning: handling missing CustomerIDs, removing duplicates, flagging cancellations
- Revenue and loss analysis, including identifying major fee/adjustment-driven losses
- Time-based analysis of sales by month and day of week
- Product-level return rate analysis to flag problem inventory
- Customer segmentation using RFM (Recency, Frequency, Monetary) scoring with quantile-based binning (`qcut`)

**Key finding:** Customers in the "Champion" segment make up only ~29% of the customer base but generate roughly 76% of total revenue, highlighting where retention efforts are best spent.

**Tools:** Python, pandas, NumPy, Matplotlib

---

### 2. Global Superstore Analysis
**File:** `Global-Superstore-analysis.ipynb`

An investigation into retail operational efficiency and managerial accountability using the Global Superstore dataset, connecting profit performance to shipping methods, returns, and regional management.

**What this project covers:**
- Merging three separate data sources (Orders, Returns, People) using left joins
- Building a net profitability model by linking returns back to individual transactions
- Manager-level performance ranking by total net profit and profit margin
- Identifying which product sub-categories drive the most loss from returns
- Comparing profit margins across shipping methods to isolate discount-driven vs. return-driven losses

**Key finding:** First Class shipping has the lowest profit margin (11.35%), driven primarily by a high discount rate (14.9%) rather than by returns, suggesting the sales team trades margin for speed to close deals.

**Tools:** Python, pandas, Matplotlib, Seaborn

---

### 3. NBA Player PER Regression
**File:** `nba_per_regression.ipynb`

A linear regression model predicting a player's next-season performance (using a simplified Player Efficiency Rating proxy) from their current-season box score statistics, with data pulled directly from the NBA Stats API.

**What this project covers:**
- Pulling and cleaning player statistics via API for two consecutive seasons
- Feature engineering an efficiency proxy from points, rebounds, assists, steals, blocks, and turnovers
- Building and evaluating a linear regression model (MAE, RMSE, R²)
- Identifying the strongest statistical predictors of future performance
- Analyzing largest prediction errors to understand model limitations

**Key finding:** The model explains roughly 71% of the variance in next-season performance (R² = 0.708), with current production and minutes played as the strongest predictors. It performs less reliably for elite, outlier-level seasons and players undergoing role or team changes.

**Tools:** Python, pandas, scikit-learn, NBA Stats API

---

## 🛠️ Tools & Technologies
- **Languages:** Python
- **Libraries:** pandas, NumPy, Matplotlib, Seaborn, scikit-learn
- **Environment:** Jupyter Notebook (via PyCharm)
- **Version Control:** Git & GitHub

## 🚀 Getting Started

Clone the repo and set up the environment:

```bash
git clone https://github.com/allenadron3-lang/Data-Analytics-Portfolio.git
cd Data-Analytics-Portfolio
python3 -m venv .venv
source .venv/bin/activate
pip install pandas numpy matplotlib seaborn scikit-learn jupyter notebook ipykernel nba_api
```

Then open any notebook in Jupyter or PyCharm.

## 📁 Data
Datasets used in these projects come from public sources (Kaggle, UCI, and the NBA Stats API). Raw data files may not be included directly in this repo due to size; see each notebook for the original source and loading instructions.

## 📬 Contact
Recent graduate seeking Data Analyst roles. Feel free to reach out via [LinkedIn](www.linkedin.com/in/adron-allen04) or [email](allenadron3@gmail.com).
