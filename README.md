# Customer Shopping Behavior Analysis & Dashboard

## Project Overview

This project focuses on analyzing real-world customer shopping data to uncover meaningful insights related to customer behavior, purchase trends, and operational performance. The objective is to transform raw shopping data into actionable insights using Exploratory Data Analysis (EDA) and interactive visual dashboards. The project combines Python-based data analysis with Power BI visualization, enabling stakeholders to make informed, data-driven decisions through intuitive dashboards and KPIs.

## Prerequisites

- Python 3.7 or higher installed on your system
- PostgreSQL database server (optional, for database integration)
- Power BI Desktop for viewing dashboards
- Jupyter Notebook for running the analysis
- Basic knowledge of Python programming and SQL queries

## Installation and Setup

### 1. Install Python
- Download and install Python 3.7 or higher from the official website: https://www.python.org/downloads/
- Ensure Python is added to your system's PATH.

### 2. Install Required Python Libraries
Run the following command in your terminal or command prompt:
```
pip install pandas numpy matplotlib seaborn SQLAlchemy psycopg2-binary
```

### 3. Install PostgreSQL (Optional)
- Download and install PostgreSQL from: https://www.postgresql.org/download/
- Set up a database and note the connection details (host, port, username, password).

### 4. Install Power BI Desktop
- Download and install Power BI Desktop from: https://powerbi.microsoft.com/desktop/

### 5. Install Jupyter Notebook
- Install Jupyter via pip:
```
pip install jupyter
```

### 6. Setup the Project
- Clone or download the project files.
- Ensure PostgreSQL is running with the appropriate database if using database connection.
- Open the notebook in Jupyter and run the cells.
- Open the Power BI file to view the dashboard.

## Usage Instructions

### Running the Jupyter Notebook
1. Launch Jupyter Notebook by running `jupyter notebook` in your terminal.
2. Navigate to the project directory and open `Banking EDA analysis.ipynb`.
3. Execute the cells sequentially to perform data loading, cleaning, analysis, and visualization.
4. Review the outputs, including plots and statistical summaries.

### Viewing the Power BI Dashboard
1. Open Power BI Desktop.
2. Load the `Banking Dashboard.pbix` file.
3. Explore the interactive dashboards, filters, and drill-through features to analyze customer segments, trends, and KPIs.

### Reviewing Reports and Presentations
- Open `Banking Exploratory Data Analysis.pdf` for a detailed report of the analysis, including charts and insights.
- Open `Banking-Exploratory-Data-Analysis-presentation.pdf` for presentation slides summarizing the project, methodology, and recommendations.

## Files

- `Banking.csv` (customer_shopping_behavior.csv): Raw dataset with customer shopping data.
- `Banking EDA analysis.ipynb` (Customer Shopping Behavior Analysis.ipynb): Jupyter Notebook for data cleaning, EDA, visualizations, and database integration using Python.
- `Banking Dashboard.pbix` (Customer_Behavior_Dashboard.pbix): Power BI dashboard file for interactive visualizations of customer segments, trends, and KPIs.
- `Banking Exploratory Data Analysis.pdf` (Customer Shopping Behavior Analysis.pdf): Detailed PDF report of the analysis, including charts and insights.
- `Banking-Exploratory-Data-Analysis-presentation.pdf` (Customer-Shopping-Behavior-Analysis_presentation.pdf): Presentation slides summarizing the project, methodology, and recommendations.

## Dataset

The dataset (`Banking.csv`) includes the following key columns:

- **Customer Demographics**: Age, Gender, Location
- **Purchase Details**: Item Purchased, Category, Purchase Amount (USD), Payment Method, Shipping Type
- **Behavioral Data**: Frequency of Purchases, Previous Purchases, Review Rating, Discount Applied, Subscription Status

## Analysis Overview

This project performs exploratory data analysis on customer shopping data. The analysis includes:

- Loading data from a CSV file and optionally from a PostgreSQL database.
- Examining data structure, descriptive statistics, and distributions.
- Analyzing categorical variables with count plots.
- Analyzing numerical variables with histograms and correlation heatmaps.
- Income banding and visualization.

## Methodologies

The project employs the following methodologies for data analysis and visualization:

- **Exploratory Data Analysis (EDA)**: Systematic approach to analyze and summarize main characteristics of the data.
- **Descriptive Statistics**: Use of mean, median, standard deviation, and other statistics to describe data distributions.
- **Data Visualization**: Creation of plots such as histograms, count plots, and heatmaps using Matplotlib and Seaborn.
- **Correlation Analysis**: Examination of relationships between numerical variables using correlation matrices and heatmaps.
- **Data Binning**: Categorization of continuous variables (e.g., income) into discrete bands for better analysis.
- **Database Querying**: SQL queries to retrieve data from PostgreSQL database for integrated analysis.

## Data Analysis Steps

The Jupyter notebook performs the following steps:

1. **Data Loading**: Load data from 'Banking.csv' using pandas.
2. **Database Integration**: Connect to PostgreSQL database and retrieve data from the 'customer' table.
3. **Initial Exploration**: Examine data structure with df.head(), df.shape, df.info(), and descriptive statistics with df.describe().
4. **Categorical Analysis**: Analyze categorical variables with value counts and count plots using Seaborn.
5. **Numerical Analysis**: Visualize numerical variables with histograms.
6. **Correlation Analysis**: Create a heatmap of the correlation matrix for numerical columns.
7. **Income Banding**: Categorize estimated income into bands (Low, Medium, High) and visualize distributions.

## Workflow and Tool Integration

The project follows a structured workflow integrating multiple tools for comprehensive data analysis:

1. **Data Extraction and Preparation**: Data is extracted from CSV files and optionally from a PostgreSQL database using Python (Pandas) and SQL queries.
2. **Data Cleaning and Transformation**: Python scripts handle data cleaning, standardization (e.g., renaming columns to snake_case), and initial processing.
3. **Exploratory Data Analysis**: Jupyter Notebook executes Python code for statistical analysis and visualization.
4. **Dashboard Development**: Processed data is used to create interactive dashboards in Power BI for stakeholder presentation.

**Tool Integration**:
- Python serves as the core for data manipulation and analysis, with libraries like Pandas for data handling, Seaborn and Matplotlib for visualizations.
- PostgreSQL provides relational database storage and querying capabilities.
- Jupyter Notebook facilitates interactive development and execution of analysis code.
- Power BI integrates the analyzed data for dynamic, user-friendly dashboards with drill-through capabilities.

The data flow can be visualized as:

SQL Database

  ↓

Python (Data Processing)

  ↓

Jupyter Notebook (Analysis)

  ↓

Power BI (Dashboard)

This integrated approach ensures data flows from raw processing to advanced analytics and visualization.

## Technologies Used

- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, SQLAlchemy, psycopg2-binary
- **Database**: PostgreSQL
- **Visualization**: Power BI, Jupyter Notebook
- **Other Tools**: SQL for querying

## Dashboard Overview

The Power BI dashboard provides interactive visualizations and insights into the customer shopping data:

- **Banking Data Analytics Dashboard**: High-level overview of key metrics including total clients, loans, deposits, fees, and account balances.
- **Loan Analysis Dashboard**: Detailed breakdown of loans across banking relationships, income bands, nationalities, and age groups.
- **Deposit Analysis Dashboard**: Comprehensive view of customer deposits across account types, income bands, and engagement timeframes.
- **Summary Dashboard**: Consolidated snapshot of customer activity, lending exposure, and deposit distribution.
- **Drill-through Analysis**: Customer-level details on fees, engagement, and credit card activity.

Key Metrics:
- Total Clients: 2,940
- Total Loan: $4.38 Bn
- Total Deposit: $3.77 Bn
- Total Fees: $158.19 M

## Key Insights

- **Customer Demographics**: Analysis of age, gender, and location distributions to understand the customer base.
- **Purchase Behavior**: Insights into item categories, purchase amounts, and frequency of purchases.
- **Payment and Shipping Preferences**: Trends in payment methods and shipping types chosen by customers.
- **Subscription and Review Analysis**: Impact of subscription status and review ratings on customer loyalty and repeat purchases.
- **Discount and Promo Effectiveness**: Evaluation of how discounts and promo codes influence purchase decisions.

## Business Recommendations

- **Targeted Marketing**: Use demographic insights to tailor marketing campaigns to specific age groups, genders, and locations for better engagement.
- **Enhance Customer Loyalty**: Encourage subscriptions by highlighting benefits, as subscribers show higher repeat purchase rates.
- **Optimize Pricing and Discounts**: Increase the use of discounts and promo codes in promotions to boost purchase amounts and frequency.
- **Improve Payment and Shipping Options**: Based on customer preferences, prioritize popular payment methods and shipping types to enhance user experience.
- **Personalize Shopping Experience**: Leverage review ratings and previous purchases to recommend products and improve customer satisfaction.

## Contributing

Contributions are welcome. Please submit issues or pull requests for improvements.

## Author

Aditi Sah

Email: aditisah2005@gmail.com
