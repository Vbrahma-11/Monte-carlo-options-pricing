# Monte Carlo Options Pricing Engine

A GPU-accelerated project that prices stock options using Monte Carlo simulation. Built with Python and PyTorch.

## What This Does

This project calculates the fair value of stock options (contracts that give you the right to buy or sell stocks at a specific price). It uses:
- **Monte Carlo Simulation**: Runs thousands of possible future scenarios
- **GPU Acceleration**: Uses your graphics card to make it fast
- **Black-Scholes Formula**: Validates results against the standard pricing model

## Features

- Price European and American options (calls and puts)
- Calculate "Greeks" (risk metrics like Delta and Gamma)
- GPU-accelerated - runs 500,000+ simulations in under a second
- Includes visualizations showing how prices change

## Requirements

- Python 3.8+
- CUDA-capable GPU (I used RTX 4070)
- These packages:
```bash
pip install torch numpy matplotlib scipy pandas
```

## How to Run

Open `options_pricing_monte_carlo.ipynb` in Jupyter Notebook and run the cells in order (1 through 8).


## What I Learned

- How Monte Carlo simulation works for financial modeling
- GPU programming with PyTorch and CUDA
- Options pricing theory (Black-Scholes model)
- The Longstaff-Schwartz algorithm for American options
- How to calculate financial risk metrics (Greeks)

## Project Structure

The notebook has 8 cells:
1. **Setup** - Import libraries and detect GPU
2. **Stock Simulation** - Generate random stock price paths
3. **European Options** - Price options that can only be exercised at expiration
4. **Black-Scholes** - Compare Monte Carlo to the exact formula
5. **Greeks** - Calculate risk sensitivities (Delta, Gamma, and more)
6. **American Options** - Price options with early exercise using LSA
7. **Sensitivity Analysis** - See how prices change with different inputs
8. **Pricing Interface** - Complete tool for pricing any option

## Why I Built This

I wanted to learn about quantitative finance and GPU programming. Options pricing is a practical application that combines probability, statistics, and financial concepts/theories.

## Future Ideas

- Add implied volatility calculator
- Support for dividend-paying stocks
- More exotic option types
- Real-time data integration

## Resources Used

- *Options, Futures, and Other Derivatives* by John Hull
- PyTorch Documentation
- QuantPy (Youtube)
- Black-Scholes and Longstaff-Schwartz papers

## Disclaimer

This is an educational project. Not intended for actual trading.

## Contact

- Vishal Brahma (Carnegie Mellon University 2029)
- GitHub: @VBrahma-11
- Email: Vbrahma@andrew.cmu.edu

Thank you for viewing and appreciating my project!
