
# Natural Gas Storage Contract Pricing Model  

A Python-based pricing model for valuing natural gas storage contracts, accounting for seasonal price variations, storage constraints, and operational costs. Built for commodity trading desks to evaluate contract profitability before execution.

## Key Features  

✅ **Comprehensive Pricing Logic**  
- Calculates contract value based on injection/withdrawal schedules, storage costs, and market prices  
- Considers all cash flows: purchase costs, sale revenue, storage fees, and transportation costs  
- Handles multiple injection/withdrawal dates with volume constraints  

✅ **Data-Driven Approach**  
- Uses historical/forecasted price data (supports CSV input)  
- Linear interpolation for dates without exact price data  

✅ **Validation & Testing**  
- Pre-configured test cases with realistic parameters  
- Visualizations comparing contract economics  
- Constraints enforcement (max storage volume, injection/withdrawal rates)  

✅ **Production-Ready Foundation**  
- OOP implementation with `StorageContractPricer` class  
- Type hints and error handling  
- Modular design for integration with trading systems  

## Technical Implementation  
- **Python 3** with pandas, numpy, statsmodels  
- Jupyter Notebook for prototyping/analysis  
- Matplotlib visualizations  

## Example Use Case  
A client wants to:  
1. Buy 50,000 MMBtu gas in May-July 2024 @ ~$2.30/MMBtu  
2. Store until winter (Dec 2024-Feb 2025)  
3. Sell at predicted ~$3.00/MMBtu  
4. Pay $10K/month storage + $0.05/MMBtu injection fees  

**Model Output:**  
```text
Net Contract Value: $-103,654.04  
Gross Profit: $32,016.13  
Total Storage Cost: $90,670.17  
[Full breakdown included]
```

## Getting Started  
1. Install dependencies:  
   ```bash
   pip install pandas numpy matplotlib statsmodels
   ```
2. Run `Natural_Gas_Price_Analysis_and_Forecasting.ipynb`  
3. Modify test cases in the "Model Usage" section  

