# Vendor Performance Analysis Project

## Project Objective

This project aims to analyze vendor performance through comprehensive data analysis of inventory, sales, purchases, and vendor invoice data. The primary goal is to evaluate vendor efficiency, profitability, and operational metrics to provide actionable insights for business decision-making.

**Key Objectives:**
- Analyze vendor performance across multiple dimensions
- Calculate profitability metrics and KPIs
- Identify top-performing vendors and areas for improvement
- Provide data-driven insights for vendor management optimization

## Dataset Used

https://drive.google.com/drive/folders/1vuUbSkvPNS7uSQIwAcSOcBbXi4imkFqq?usp=drive_link

## Questions (KPIs)

The analysis addresses the following key performance indicators and business questions:

### Financial Performance Metrics:
- **Gross Profit**: Sales revenue minus purchase costs
- **Profit Margin**: Percentage of profit relative to sales revenue
- **Sales to Purchase Ratio**: Efficiency of sales relative to inventory purchases

### Operational Efficiency Metrics:
- **Stock Turnover**: Rate of inventory movement (sales quantity / purchase quantity)
- **Freight Cost Analysis**: Transportation expenses by vendor
- **Inventory Management**: Beginning vs ending inventory levels

### Vendor Performance Questions:
1. Which vendors generate the highest gross profit?
2. What is the profit margin by vendor and brand?
3. How efficient is each vendor in terms of stock turnover?
4. Which vendors have the highest freight costs relative to sales?
5. What is the sales-to-purchase ratio for each vendor?
6. Which brands perform best across different vendors?

## Process

### Data Pipeline Architecture:

1. **Data Ingestion** (`ingestion_db.py`)
   - Loads CSV files from the data directory
   - Processes data in chunks for memory efficiency
   - Ingests data into SQLite database (`inventory.db`)
   - Implements logging for process monitoring

2. **Data Processing** (`get_vendor_summary.py`)
   - Creates comprehensive vendor summary through SQL queries
   - Merges multiple tables (purchases, sales, vendor_invoice, purchase_prices)
   - Calculates derived metrics and KPIs
   - Cleans and prepares data for analysis

3. **Analysis Workflow**:
   - **Exploratory Data Analysis** (`Exploratory Data Analysis.ipynb`)
   - **Vendor Performance Analysis** (`Vendor Performance Analysis.ipynb`)
   - **Logging and Monitoring** (`logging.ipynb`)

### Technical Implementation:
- **Database**: SQLite for data storage and querying
- **Data Processing**: Pandas for data manipulation and analysis
- **Logging**: Comprehensive logging system for process tracking
- **Chunked Processing**: Handles large datasets efficiently

## Dashboard Project Insight

Dashboard Link:file:///C:/Users/ASUS/AppData/Local/Temp/Power%20BI%20Desktop/print-job-de50d5fe-2aef-4a92-ae40-a3fd9cece4ae/Vendor%20Performance%20Dashboard.pdf

The project generates comprehensive insights through:

### Key Metrics Dashboard:
- **Vendor Performance Rankings**: Top vendors by various metrics
- **Profitability Analysis**: Gross profit and margin visualizations
- **Operational Efficiency**: Stock turnover and sales ratios
- **Cost Analysis**: Freight costs and purchase efficiency

### Analytical Insights:
- Vendor profitability comparisons
- Brand performance across vendors
- Inventory management efficiency
- Cost structure analysis
- Performance trend identification

### Visualization Components:
- Performance comparison charts
- Profitability heatmaps
- Efficiency scatter plots
- Cost breakdown visualizations


## Final Conclusion

### Key Findings:

1. **Vendor Performance Variation**: Significant differences in vendor profitability and efficiency metrics
2. **Profit Margin Insights**: Clear identification of high and low-margin vendors
3. **Operational Efficiency**: Stock turnover rates vary considerably across vendors
4. **Cost Structure Analysis**: Freight costs impact overall vendor profitability
5. **Brand Performance**: Certain brands perform consistently better across vendors

### Business Impact:

- **Vendor Optimization**: Identifies opportunities for vendor consolidation or diversification
- **Pricing Strategy**: Insights into pricing efficiency and margin optimization
- **Inventory Management**: Recommendations for stock level optimization
- **Cost Control**: Freight cost analysis for logistics optimization

### Recommendations:

1. **Focus on High-Performing Vendors**: Prioritize relationships with vendors showing strong profitability metrics
2. **Optimize Low-Performing Relationships**: Develop improvement plans for vendors with poor performance
3. **Inventory Strategy**: Adjust stock levels based on turnover analysis
4. **Cost Management**: Negotiate better freight terms with high-cost vendors
5. **Data-Driven Decisions**: Use insights for strategic vendor management decisions

### Technical Achievements:

- Successfully processed large-scale datasets (1.5GB+ total)
- Implemented efficient data pipeline with chunked processing
- Created comprehensive vendor performance metrics
- Established robust logging and monitoring system
- Generated actionable business insights through data analysis

This project demonstrates the power of data-driven vendor management and provides a foundation for ongoing performance monitoring and optimization. 