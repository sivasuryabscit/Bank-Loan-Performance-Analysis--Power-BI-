# Bank Loan Performance Analysis

A comprehensive Power BI dashboard analyzing loan performance and borrower characteristics for banking institutions.

## 📊 Project Overview
This project analyzes lending loan data to uncover relationships between borrower behavior and loan characteristics, providing actionable insights for optimizing loan lending strategies and mitigating credit risk.

## 🎯 Key Features
- **Loan Performance Analysis**: Track funding, repayment rates, and performance metrics
- **Borrower Profile Analysis**: Analyze demographics, income, and risk factors
- **Interactive Dashboards**: Dynamic filtering and cross-visual interactions
- **Risk Assessment**: Delinquency tracking and verification status analysis

## 📈 Key Metrics
- Total Funded Amount: $6,630.19 Million
- Fully Paid Loan Percentage: 3962.1%
- Average Interest Rate by Term
- Loan Distribution by Purpose and Status

## 🛠️ Technologies Used
- **Power BI Desktop**: Data visualization and reporting
- **Power Query**: Data cleaning and transformation
- **DAX**: Custom calculations and measures
- **Excel**: Source data format

## 📁 Project Structure
- `data/`: Raw dataset and data dictionary
- `reports/`: Power BI files (.pbix) and screenshots
- `themes/`: Custom JSON theme for consistent styling

## 🚀 How to Use
1. Download Power BI Desktop (free)
2. Clone this repository
3. Open `reports/Bank_Loan_Performance_Analysis.pbix`
4. Apply custom theme from `themes/BankLoanTheme.json`
5. Explore the interactive dashboards

## 📊 Dashboard Screenshots
### Report 1: Loan Performance Analysis
![Loan Performance](reports/screenshots/report1_loan_performance.png)

### Report 2: Borrower Profile Analysis  
![Borrower Profile](reports/screenshots/report2_borrower_profile.png)

## 🔍 Key Insights
- [Add your key findings here]
- [Performance patterns discovered]
- [Risk factors identified]

## 📋 DAX Formulas Used
- **Remaining Installments**: `CEILING(BorrowerDetails[out_prncp] / RELATED(LoanDetails[installment]), 1)`
- **Non-Verified Borrowers Count**: `COUNTROWS(FILTER(BorrowerDetails, BorrowerDetails[verification_status] = "Not Verified"))`
- **Fully Paid Loan Percentage**: `DIVIDE(COUNTROWS(FILTER(LoanDetails, LoanDetails[loan_status] = "Fully Paid")), COUNTROWS(LoanDetails)) * 100`

## 🤝 Contributing
Feel free to fork this project and submit pull requests for improvements.

## 📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author
[Your Name]
- LinkedIn: [Your LinkedIn]
- Email: [Your Email]

## 🙏 Acknowledgments
- Dataset source: [Credit the data source]
- Inspired by real-world banking analytics needs
