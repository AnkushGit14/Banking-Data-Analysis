# Banking Data Analysis

## Project Overview
This project involves an Exploratory Data Analysis (EDA) of a banking dataset to uncover insights into customer demographics, financial behaviors, and relationships between various banking products. The analysis aims to understand the dataset's structure, identify patterns, and prepare the data for further modeling or reporting.

## Dataset
The dataset used for this analysis is `Banking.csv`. It contains 3000 entries and 25 columns, providing a comprehensive view of bank clients.

**Key Columns include:**
* `Client ID`: Unique identifier for each client.
* `Name`: Client's name.
* `Age`: Client's age.
* `Location ID`: Identifier for the client's location.
* `Joined Bank`: Date when the client joined the bank.
* `Banking Contact`: Name of the client's banking contact.
* `Nationality`: Client's nationality.
* `Occupation`: Client's occupation.
* `Fee Structure`: Fee structure applied to the client (e.g., High, Mid, Low).
* `Loyalty Classification`: Client's loyalty status (e.g., Jade, Silver, Gold, Platinum).
* `Estimated Income`: Client's estimated annual income.
* `Superannuation Savings`: Client's superannuation savings.
* `Amount of Credit Cards`: Number of credit cards held by the client.
* `Credit Card Balance`: Balance on credit cards.
* `Bank Loans`: Amount of bank loans.
* `Bank Deposits`: Total bank deposits.
* `Checking Accounts`: Balance in checking accounts.
* `Saving Accounts`: Balance in saving accounts.
* `Foreign Currency Account`: Balance in foreign currency accounts.
* `Business Lending`: Amount of business lending.
* `Properties Owned`: Number of properties owned by the client.
* `Risk Weighting`: Risk weighting assigned to the client.
* `BRId`, `GenderId`, `IAId`: Additional identification columns.

## Analysis Performed

The exploratory data analysis covered the following aspects:

1.  **Data Loading and Initial Inspection**:
    * Loaded the `Banking.csv` file into a Pandas DataFrame.
    * Inspected the first few rows using `df.head()`.
    * Checked the shape of the DataFrame (`df.shape`) to understand the number of rows and columns.
    * Obtained a concise summary of the DataFrame using `df.info()` to check data types and non-null counts.

2.  **Descriptive Statistics**:
    * Generated descriptive statistics for numerical columns using `df.describe()` to understand central tendency, dispersion, and shape of the distributions.

3.  **Missing Values**:
    * Verified the absence of missing values across all columns, confirming data completeness.

4.  **Data Type Conversion**:
    * Converted the 'Joined Bank' column to datetime objects for proper temporal analysis.

5.  **Feature Engineering**:
    * Created a new categorical feature 'Income Band' by grouping 'Estimated Income' into 'Low', 'Mid', and 'High' categories.

6.  **Categorical Variable Analysis**:
    * Examined the distribution of unique categories for key categorical columns:
        * 'Risk Weighting'
        * 'Nationality'
        * 'Occupation'
        * 'Fee Structure'
        * 'Loyalty Classification'
        * 'Properties Owned'
        * 'Income Band'
    * Used `value_counts()` and visualizations (histograms, bar plots) to understand the frequency of each category.

7.  **Correlation Analysis**:
    * Calculated the correlation matrix for numerical features to identify relationships between variables.
    * Visualized correlations using a heatmap (`seaborn.heatmap`) for better interpretability.

8.  **Visualizations**:
    * Utilized `matplotlib.pyplot` and `seaborn` for various plots, including:
        * Histograms to visualize the distribution of numerical features like 'Age', 'Estimated Income', 'Bank Deposits', etc.
        * Box plots to identify outliers and compare distributions across different categories.
        * Bar plots for categorical variable distributions.
        * Scatter plots to explore relationships between two numerical variables.

## Key Findings & Insights
* **Income Distribution**: The 'Income Band' feature revealed a distribution where a significant portion of clients fall into the 'Mid' income category, followed by 'Low' and then 'High'.
* **Customer Demographics**: The analysis provided insights into the distribution of clients by nationality, occupation, and age.
* **Financial Product Usage**: Relationships between different financial products (e.g., Bank Loans, Credit Card Balance, Savings, Checking) reflect common financial lifecycle trends: higher income earners and older individuals often accumulate more savings, retirement funds, and may carry higher credit card balances or loans.
* **Low Correlation with Properties Owned**: Property ownership showed weaker correlations with banking variables, suggesting external factors (location, real estate market conditions, inheritance, etc.) not captured by the dataset might play a larger role.
* **Business vs. Personal Banking**: Business Lending showed a moderate link to Bank Loans, indicating some customers might have both personal and business debts. However, business lending was relatively uncorrelated with other deposit or property-related metrics, suggesting it may serve a distinct subset of customers or needs.

## Technologies Used
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

## How to Run the Project

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone <your-repo-url>
    cd banking-data-analysis
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Place the dataset:**
    Ensure `Banking.csv` is in the root directory of the project.
5.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook BankEDA\ \(Version\ 2\).ipynb
    ```
    (You can also open `BankEDA (Version 1).ipynb` if you prefer to see the initial stages of the analysis.)

This will open the Jupyter Notebook interface in your browser, where you can run the cells and explore the analysis.
