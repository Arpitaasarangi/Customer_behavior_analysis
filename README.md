# 🛍️Customer_behavior_analysis
 This project explores customer shopping behavior using transactional data from 3,900 purchases across various product categories. It combines Python for data cleaning and feature engineering, SQL for business-driven analytics, Power BI for interactive dashboard visualization and final report presentation using Gamma.
 
**Dataset**:
- Size: 3,900 rows × 18 columns

 **Features**:
- Customer demographics: Age, Gender, Location, Subscription Status
- Purchase details: Item, Category, Amount, Season, Size, Color
- Behavior indicators: Discounts, Promo Codes, Frequency, Reviews, Shipping Type

**Tools and Technologies used**:
- python: Data loading, cleaning, EDA(Exploratory Data Analysis)
- MYSQL: Business logic & SQL queries
- Power Bi: Dashboard Creation
- Gamma: Final report presentation

🔄**Project Workflow**:
1. Data Preparation (Python)
- Loaded dataset using pandas
- Explored structure with .info() and .describe()
- Imputed missing review ratings by product category median
- Standardized column names to snake_case
- Engineered new features:
- age_group (binned age ranges)
- purchase_frequency_days (from purchase history)
- Dropped redundant columns after consistency checks
- Loaded cleaned data into MySQL for analysis
  
2.🛢️Business Analysis (SQL)
- Revenue comparison by gender and subscription status
- High-spending discount users
- Top-rated products
- Shipping type impact on spend
- Discount dependency by product
- Customer segmentation: New, Returning, Loyal
- Age group revenue contribution

3.📊Dashboard (Power BI)
- Visualized key metrics:
- Average spend, review ratings, subscription split
- Revenue by category, age group, shipping type
- Customer segmentation and product performance

4. Final Report (Gamma)
- Summarized insights and recommendations
- Presented findings in a clean, interactive format

📈 Dashboard Highlights
- Average Purchase Amount: $59.76
- Average Review Rating: 3.75
- Subscription Split: 27% Yes, 73% No
- Top Revenue Contributors: Young Adults, Male Customers
- Most Purchased Items: Blouse, Jewelry, Sandals
- High Discount Usage: Hat, Sneakers, Coat

🚀 How to Run
- Clone the repository
git clone https://github.com/your-username/customer-behavior-analysis.git
- Set up Python environment
- Install dependencies: pip install -r requirements.txt
- Run the Jupyter notebook
- Navigate to notebooks/Customer_Analysis.ipynb
- Load cleaned data into MySQL
- Use sql/load_data.sql to import
- Execute SQL queries
- Run sql/Customer_analysis_queries.sql in MySQL Workbench or CLI
- Open Power BI dashboard
- File: dashboard/cust_analysis.pbix
- View final report


