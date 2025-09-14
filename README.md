# Customer Segmentation - RFM Analysis

A comprehensive customer segmentation analysis using RFM (Recency, Frequency, Monetary) methodology to categorize customers and derive actionable business insights from e-commerce transaction data.

## Overview

This project performs customer segmentation analysis on an online retail dataset using the RFM (Recency, Frequency, Monetary) model. The analysis helps businesses understand customer behavior patterns and develop targeted marketing strategies.

## What is RFM Analysis?

RFM analysis is a customer segmentation technique that uses three key metrics:

- **Recency (R)**: How recently a customer made a purchase
- **Frequency (F)**: How often a customer makes purchases
- **Monetary (M)**: How much money a customer spends

## Features

- **Data Preprocessing**: Cleans and prepares transaction data for analysis
- **RFM Calculation**: Computes Recency, Frequency, and Monetary values for each customer
- **Customer Scoring**: Assigns RFM scores based on quantile-based scoring system
- **Customer Segmentation**: Categorizes customers into distinct segments:
  - **Best Customers**: High RFM scores (≥9) - most valuable customers
  - **Loyal Customers**: Medium-high RFM scores (6-8) - regular customers
  - **At Risk**: Medium-low RFM scores (4-5) - customers showing declining engagement
  - **Low-Value**: Low RFM scores (<4) - least engaged customers
- **Data Visualization**: Creates informative plots showing customer distribution and behavior patterns
- **Business Insights**: Provides actionable recommendations for each customer segment

## Technologies Used

- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Matplotlib**: Static plotting and visualization
- **Seaborn**: Statistical data visualization
- **Jupyter Notebook**: Interactive development environment

## Dataset

The analysis is performed on the Online Retail dataset containing:
- **541,909 transactions** from UK-based online retailer
- **8 columns**: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country
- **Time period**: Transactions from 2010-2011
- **Customer coverage**: 4,372 unique customers

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Dhwani123p/Customer-Segmentation-Using-RFM-Analysis.git
cd Customer-Segmentation-Using-RFM-Analysis
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Open the Jupyter notebook:
```bash
jupyter notebook customer-segmentation-rfm-analysis.ipynb
```

## Usage

### Running the Analysis

1. **Data Loading**: Load the Online Retail dataset
2. **Data Cleaning**: Remove invalid transactions and handle missing values
3. **RFM Calculation**: Compute Recency, Frequency, and Monetary metrics
4. **Scoring**: Assign RFM scores using quantile-based methodology
5. **Segmentation**: Categorize customers into business-relevant segments
6. **Visualization**: Create plots to understand customer distribution
7. **Insights**: Generate actionable business recommendations

### Key Metrics Calculated

- **Recency**: Days since last purchase (lower is better)
- **Frequency**: Number of unique invoices (higher is better)
- **Monetary**: Total amount spent (higher is better)

### Customer Segments

| Segment | RFM Score | Characteristics | Strategy |
|---------|-----------|----------------|----------|
| Best Customers | ≥9 | Recent, frequent, high-value | Retain with premium services |
| Loyal Customers | 6-8 | Regular customers with good value | Upsell and cross-sell |
| At Risk | 4-5 | Showing declining engagement | Re-engagement campaigns |
| Low-Value | <4 | Least engaged customers | Win-back campaigns or cost reduction |

## Results

The analysis reveals customer distribution and behavior patterns:

- **Best Customers (1,619)**: 36.9% of customer base, highest lifetime value
- **Loyal Customers (1,316)**: 30.1% of customer base, consistent purchasers
- **At Risk (962)**: 22.0% of customer base, need immediate attention
- **Low-Value (442)**: 10.1% of customer base, minimal engagement

## Business Applications

### Marketing Strategies
- **Personalized Campaigns**: Target each segment with appropriate messaging
- **Retention Programs**: Focus on At Risk customers to prevent churn
- **Loyalty Programs**: Reward Best and Loyal customers
- **Win-back Campaigns**: Re-engage Low-Value customers

### Revenue Optimization
- **Cross-selling**: Identify opportunities among Loyal customers
- **Upselling**: Target Best customers with premium products
- **Pricing Strategies**: Segment-based pricing approaches
- **Inventory Management**: Align stock with customer preferences

## Customization

You can customize the analysis by:
- **Adjusting RFM thresholds** for different scoring systems
- **Modifying segment definitions** based on business needs
- **Adding additional metrics** like product categories or geographic data
- **Changing visualization styles** and color schemes
- **Incorporating time-based analysis** for trend identification

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Online Retail dataset for providing real-world transaction data
- RFM methodology for customer segmentation framework
- Python data science ecosystem for analysis tools

## Future Enhancements

- [ ] Advanced segmentation algorithms (K-means clustering)
- [ ] Predictive modeling for customer lifetime value
- [ ] Real-time segmentation dashboard
- [ ] Integration with CRM systems
- [ ] A/B testing framework for segment-based campaigns
