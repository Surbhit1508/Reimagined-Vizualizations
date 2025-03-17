# Reimagined-Vizualizations
# Order Source Analysis Project

## Overview
This project analyzes order data from multiple sources across Texas and Arkansas. It combines order statistics with demographic data to uncover insights into purchasing patterns, regional differences, and market performance across zip codes.

## Table of Contents
- [Features](#features)
- [Data Sources](#data-sources)
- [Installation](#installation)
- [Usage](#usage)
- [Data Analysis Workflow](#data-analysis-workflow)
- [Visualizations](#visualizations)
- [Key Insights](#key-insights)
- [Dependencies](#dependencies)
- [License](#license)

## Features
- Merges order data with demographic information by zip code
- Analyzes order patterns by state, order source, and zip code
- Calculates key metrics such as average order amounts and total revenue
- Creates interactive visualizations of business performance
- Generates executive-level summary reports

## Data Sources
The analysis uses two primary data sources:
1. **Order_Source_Stats_By_Zip.csv** - Contains order information including:
   - Zip Code
   - Customer State
   - Order Source (Fax, Phone, Web)
   - Total Order Amount
   - Average Order Amount
   - Unique Orders

2. **Zip_Code.json** - Contains demographic information by zip code:
   - Population statistics
   - Income data
   - Housing information
   - Age distribution
   - Education metrics
   - Employment figures

## Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/order-source-analysis.git
cd order-source-analysis

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Usage
1. Place your data files in the project directory:
   - `Order_Source_Stats_By_Zip.csv`
   - `Zip_Code.json`

2. Run the main analysis script:
```bash
python order_analysis.py
```

3. Generated visualizations will be saved in the project directory:
   - `order_analysis_visualization.png`
   - `interactive_revenue_dashboard.html`
   - `business_performance_summary.png`

## Data Analysis Workflow
1. **Data Loading & Exploration**
   - Load order statistics and zip code demographic data
   - Explore basic statistics and data structure
   - Check for missing values and data types

2. **Data Preprocessing**
   - Merge datasets on zip code
   - Handle any missing or inconsistent data
   - Create derived metrics

3. **Statistical Analysis**
   - Calculate summary statistics by state and order source
   - Analyze correlations between demographic factors and order patterns
   - Identify key performance indicators

4. **Visualization & Reporting**
   - Create comprehensive visualizations for analysis
   - Generate executive-level performance summaries
   - Build interactive dashboards

## Visualizations
The project generates several visualization types:

1. **Professional Analysis Dashboard**
   - Distribution of average order amounts
   - State revenue comparison
   - Correlation matrix of key metrics
   - Summary statistics table

2. **Interactive Revenue Dashboard**
   - Time-series revenue analysis
   - Order volume trends
   - Rolling averages
   - Interactive elements for exploration

3. **Executive Business Summary**
   - Revenue by state
   - Order distribution
   - Key performance indicators
   - Business insights table

## Key Insights
- Texas generates approximately **86.3%** of total revenue, with Arkansas accounting for **13.7%**
- Total revenue across both markets: **$1,558,927.83**
- Average order value: **$1,294.36**
- Orders are processed through three channels: Web, Phone, and Fax
- Data covers **129 zip codes** across two states
- The distribution of average order amounts follows a normal distribution
- Moderate correlation between household income and average order amount

## Dependencies
- Python 3.6+
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- datetime

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## Contact
For questions or feedback, please contact [surbhit@uark.edu](mailto:surbhit@uark.edu).
