# 📊 Fixed Income Portfolio Analysis - MIAX Module 2

**Master en Ingeniería y Análisis Financiero Quantitativo (MIAX)**  
*Módulo 2: Introducción a los Sistemas Financieros - Renta Fija*

## 🎯 Project Overview

This project involves a comprehensive analysis of a fixed income universe, specifically corporate bonds, including portfolio construction and risk management. The analysis covers bond valuation, spread calculation, duration and convexity metrics, portfolio optimization, and hedging strategies.

## 📁 Project Structure

```
├── data/
│   ├── universo.csv                    # Bond universe with essential characteristics
│   ├── precios_historicos_universo.csv # Historical closing prices for bond universe
│   ├── curvaESTR.csv                   # €STR interest rate curve
│   └── precios_historicos_varios.csv   # Historical prices for other indices
├── src/
│   ├── TallerRF_AnálisisCartera_Enunciado.ipynb  # Main analysis notebook
│   ├── tools.py                        # Utility functions and tools
│   ├── Visualizations.ipynb           # Data visualization notebook
│   └── visualizaton_analysis.py       # Visualization analysis script
├── requirements.txt                    # Python dependencies
└── entrega.txt                        # Delivery instructions
```

## 📊 Data Sources

### Bond Universe Data
- **universo.csv**: Complete bond characteristics including issuer, maturity, coupon, rating, etc.
- **precios_historicos_universo.csv**: Historical closing prices for all bonds in the universe

### Market Data
- **curvaESTR.csv**: €STR interest rate curve for bond valuation
- **precios_historicos_varios.csv**: Additional market indices including:
  - Credit indices: ITRAXX Main and ITRAXX XOVER (for credit risk hedging)
  - Interest rate futures: Schatz (DU1), BOBL (OE1), and BUND (RX1) (for interest rate hedging)
  - Credit index: RECMTREU (portfolio benchmark)

## 🔬 Analysis Components

### 1. Data Analysis & Cleaning
- Comprehensive analysis of bond characteristics
- Data cleaning and preparation for modeling
- Statistical analysis of the bond universe

### 2. Bond Valuation
- Bond pricing using discount curves
- Comparison with market prices
- Spread calculation over the yield curve

### 3. Risk Metrics
- Yield calculation
- Duration analysis
- Convexity measurement

### 4. Portfolio Construction
- **Equal-weighted portfolio**: All bonds with equal allocation
- **Optimized portfolio**: Maximum 20 bonds with constraints:
  - Duration ≤ 3 years
  - High Yield exposure ≤ 10%
  - No subordinated debt
  - Minimum issue size: €500M
  - Maximum single issue allocation: 10%
  - Maximum issuer concentration: 15%

### 5. Risk Management
- Interest rate hedging strategies
- Credit risk hedging approaches
- Portfolio risk measurement and monitoring

### 6. Performance Analysis
- Backtesting strategies
- Benchmark comparison (RECMTREU index)
- Risk-adjusted performance metrics

## 🛠️ Technical Requirements

### Dependencies
The project requires several Python packages for financial analysis:
```bash
pip install -r requirements.txt
```

Key packages include:
- `pandas`, `numpy` - Data manipulation and analysis
- `matplotlib`, `seaborn` - Data visualization
- `scipy` - Scientific computing
- `arch` - Financial econometrics
- Additional financial and statistical libraries

### Environment Setup
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Launch Jupyter: `jupyter notebook` or `jupyter lab`
4. Open the main analysis notebook: `src/TallerRF_AnálisisCartera_Enunciado.ipynb`

## 📈 Key Features

- **Comprehensive Bond Analysis**: Complete evaluation of corporate bond characteristics
- **Advanced Valuation Models**: Sophisticated pricing using yield curves
- **Risk Management**: Duration, convexity, and credit risk analysis
- **Portfolio Optimization**: Constrained optimization for optimal allocation
- **Hedging Strategies**: Interest rate and credit risk hedging techniques
- **Performance Analytics**: Backtesting and benchmark comparison

## 🎓 Learning Objectives

This project demonstrates:
- Fixed income security analysis and valuation
- Portfolio construction with real-world constraints
- Risk management in bond portfolios
- Quantitative finance techniques in Python
- Financial data analysis and visualization

## 📝 Assignment Guidelines

- **Team Size**: Up to 3 people
- **Delivery Date**: November 27th
- **Format**: Jupyter notebook with complete analysis and documentation

## 🔗 Repository Information

- **Owner**: piettro
- **Repository**: Master-MIAX-Tarea-Bloque2-Renta-Fija
- **Branch**: main

---

*This project is part of the Master in Financial Engineering and Quantitative Analysis (MIAX) curriculum, specifically Module 2 covering Introduction to Financial Systems with a focus on Fixed Income instruments.*