# MMF1941 Dynamic Data Science Project: Dynamic Shrinkage Method for Hierarchical Risk Parity (DS-HRP)

## Overview
This repository contains the code and research paper for the project **"Dynamic Shrinkage Method for Hierarchical Risk Parity to Improve Portfolio Stability and Performance"** developed for the **MMF1941 Dynamic Data Science** course at the University of Toronto.

The project introduces a novel portfolio optimization approach, **Dynamic Shrinkage Hierarchical Risk Parity (DS-HRP)**, designed to enhance the traditional **Hierarchical Risk Parity (HRP)** method by incorporating dynamic shrinkage in the covariance matrix estimation. This method improves portfolio robustness, reduces estimation errors, and enhances performance, especially in volatile and high-dimensional financial markets.

## Project Structure
```
📦 DS-HRP
├── 📄 Dynamic_Shrinkage.pdf     # Research paper explaining the methodology and results
├── 📄 code_py.ipynb             # Python code for implementing the DS-HRP model
├── 📂 data                      # (Optional) Folder for data used in the project
└── 📄 README.md                 # Project overview and instructions
```

## Key Concepts

- **Hierarchical Risk Parity (HRP):** A clustering-based portfolio optimization technique that avoids inverting the covariance matrix, addressing the instability of traditional mean-variance optimization.  
- **Dynamic Shrinkage:** An adaptive approach to adjust the covariance matrix by shrinking eigenvalues based on market conditions, improving portfolio stability.  
- **Covariance Matrix Estimation:** DS-HRP introduces a cluster-specific shrinkage factor to stabilize covariance matrices, mitigating noise and enhancing risk distribution.  
- **Monte Carlo Simulations:** Used to evaluate the performance of DS-HRP against standard HRP and Markowitz’s Critical Line Algorithm (CLA) across various market scenarios.


## Methodology

1. **Hierarchical Clustering:** Groups assets based on their pairwise correlations to build a hierarchical tree.  
2. **Dynamic Covariance Shrinkage:** Adjusts the covariance matrix dynamically to minimize the influence of unstable eigenvalues.  
3. **Quasi-Diagonalization:** Reorders the covariance matrix to isolate within-cluster correlations, improving stability.  
4. **Recursive Bisection:** Allocates capital proportionally to risk across clusters.  
5. **Performance Evaluation:** Assesses Sharpe Ratio, volatility, and maximum drawdown through backtesting on cryptocurrency datasets.


## Results

- **Enhanced Stability:** DS-HRP achieved more stable portfolio allocations compared to standard HRP and CLA, especially during periods of market volatility.  
- **Superior Performance:** The model delivered higher Sharpe Ratios and reduced portfolio concentration risk.  
- **Robust to Market Changes:** Outperformed traditional models under extreme market conditions by dynamically adjusting to asset correlations.


## Getting Started

### Prerequisites

Install required Python packages:

```bash
pip install numpy pandas matplotlib scipy scikit-learn yfinance
```

### Running the Code

1. Open the `code_py.ipynb` Jupyter Notebook.  
2. Load the dataset (or connect to a data source like Bloomberg).  
3. Run the cells to execute the DS-HRP model and analyze the results.


## Authors

- **Xinyi Shen** – Master of Mathematical Finance (MMF), University of Toronto  
- **Hamid Ariana** – York University  
- **Luis Seco** – University of Toronto  


## Acknowledgments

- **University of Toronto** – MMF1941 Dynamic Data Science Course  
- **RiskLab AI** – Research support  


## License

This project is licensed under the MIT License.

---

Let me know if you'd like any edits or additional sections!
