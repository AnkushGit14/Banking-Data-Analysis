# Banking Customer Data Analysis & EDA 🏦

A comprehensive Exploratory Data Analysis (EDA) of banking customer data to uncover insights into customer demographics, financial behaviors, and relationships between various banking products. This analysis provides actionable insights for customer segmentation, risk assessment, and product recommendations.

## 🚀 Project Overview

This project analyzes a comprehensive banking dataset to provide insights into:
- Customer demographic patterns and segmentation
- Financial product usage and preferences
- Income distribution and spending behaviors
- Risk assessment and loyalty classification
- Correlation analysis between banking products
- Customer lifetime value indicators

## 📈 Key Insights

- **Customer Segmentation**: Identified distinct customer profiles based on income, age, and product usage
- **Product Correlation**: Discovered relationships between different banking products and services
- **Risk Patterns**: Analyzed risk weighting distributions across customer segments
- **Loyalty Analysis**: Customer loyalty classification and retention patterns
- **Income Distribution**: Segmented customers into Low, Mid, and High income bands

## 🛠️ Technologies Used

- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Statistical data visualization
- **Jupyter Notebook**: Interactive development environment

## 📁 Project Structure

```
Banking-Data-Analysis/
│
├── data/
│   └── Banking.csv                   # Customer dataset (3000 records, 25 features)
│
├── notebooks/
│   ├── BankEDA (Version 1).ipynb    # Initial exploratory analysis
│   ├── BankEDA (Version 2).ipynb    # Enhanced analysis with visualizations
│   └── data_insights.ipynb          # Key findings and recommendations
│
├── src/
│   ├── data_processor.py            # Data cleaning and preprocessing
│   ├── feature_engineering.py       # Custom feature creation
│   └── visualizer.py                # Plotting functions
│
├── images/
│   ├── correlation_heatmap.png
│   ├── income_distribution.png
│   ├── customer_demographics.png
│   └── product_analysis.png
│
├── requirements.txt                  # Project dependencies
├── README.md                        # Project documentation
└── LICENSE                          # GNU GPL v3.0 License

```

## 📊 Dataset Overview

**Dataset**: `Banking.csv` with **3,000 customers** and **25 features**

### Key Features:
- **Demographics**: Age, Nationality, Occupation, Location
- **Financial Profile**: Estimated Income, Bank Deposits, Savings, Checking Accounts
- **Products**: Credit Cards, Bank Loans, Business Lending, Foreign Currency Accounts
- **Classification**: Risk Weighting, Loyalty Status, Fee Structure
- **Assets**: Properties Owned, Superannuation Savings

## 🔍 Analysis Highlights

### 1. Data Quality Assessment
- **Complete Dataset**: Zero missing values across all 25 columns
- **Data Types**: Mixed numerical and categorical variables
- **Temporal Analysis**: Customer joining patterns over time

### 2. Customer Demographics
- **Age Distribution**: Comprehensive age group analysis
- **Geographic Spread**: Location-based customer concentration
- **Occupation Patterns**: Professional distribution across banking services
- **Nationality Insights**: International customer base analysis

### 3. Financial Behavior Analysis
- **Income Segmentation**: Created Low/Mid/High income bands
- **Product Usage**: Cross-selling opportunities identification
- **Spending Patterns**: Credit card usage vs income correlation
- **Investment Behavior**: Savings and deposit patterns

### 4. Risk & Loyalty Assessment
- **Risk Weighting**: Customer risk profile distribution
- **Loyalty Classification**: Jade, Silver, Gold, Platinum tier analysis
- **Retention Factors**: Correlation between loyalty and financial products

## 📈 Key Visualizations

1. **Correlation Heatmap** - Relationships between numerical features
2. **Income Distribution Charts** - Customer segmentation visualization
3. **Product Usage Analysis** - Banking product adoption patterns  
4. **Demographics Dashboard** - Age, nationality, and occupation insights
5. **Risk Assessment Plots** - Customer risk profile visualization

## 💡 Business Insights

### Customer Segmentation Findings:
- **Mid-income customers** represent the largest segment
- Strong correlation between **age and savings** behavior
- **Higher income customers** show increased credit product usage

### Product Relationships:
- Positive correlation between **bank deposits and checking accounts**
- **Business lending** serves distinct customer subset
- **Property ownership** influenced by external market factors

### Risk & Loyalty Patterns:
- **Loyalty classification** strongly linked to product diversity
- **Risk weighting** varies significantly across income bands
- **Fee structure** optimization opportunities identified

## 🎯 Recommendations

1. **Targeted Marketing**: Develop income-band specific product campaigns
2. **Cross-selling Strategy**: Leverage product correlation insights
3. **Risk Management**: Implement dynamic risk assessment models
4. **Customer Retention**: Focus on loyalty tier progression strategies

## 🔧 Installation & Usage

```bash
# Clone repository
git clone https://github.com/AnkushGit14/Banking-Data-Analysis.git
cd Banking-Data-Analysis

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run analysis
jupyter notebook "BankEDA (Version 2).ipynb"
```

## 📝 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

**Ankush** - [thisisankushjaiswal@gmail.com](mailto:thisisankushjaiswal@gmail.com)

**Project Link**: [https://github.com/AnkushGit14/Banking-Data-Analysis](https://github.com/AnkushGit14/Banking-Data-Analysis)

---

⭐ **If you found this project helpful, please give it a star!** ⭐
