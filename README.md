# Strategy Backtesting Framework for Smart Order Routing (SOR)

Welcome to the repository for a working prototype of a **Strategy Backtesting Framework for Smart Order Routing (SOR)**. This project is designed as a practical playground for testing and analyzing trade execution strategies, especially focused on market and crypto assets across multiple trading venues.

## What is This?

In a landscape where order execution quality truly matters, this repository offers a simulation toolkit to:
- Generate realistic multi-venue market data
- Simulate order execution (using strategies such as TWAP)
- Benchmark performance against common reference prices (VWAP)
- Visualize results

While this framework is meant for demonstration and educational purposes, the modular code lets you swap in different strategies or expand data features as needed.

## Repository Structure

You’ll find the following main files:
- **work_trial_task_namit_shrivastava.py**  
  Core Python source code: orchestrates the generation of synthetic market data, defines trading strategies, runs simulations, and outputs performance metrics and plots.
- **Work_Trial_Task_Namit_Shrivastava.ipynb**  
  Jupyter notebook version for interactive exploration: contains code cells and, if you run it, will plot and print strategy analytics inline.
- **Python Code Logic Report_Namit Shrivastava.pdf**  
  High-level documentation or explanation of the Python logic.
- **Work Trial Task_Namit Shrivastava.pdf**  
  Additional supporting document—possibly describing requirements or design.
- **README.md**  
  (This file) Describes the project and how to use it.

## Main Features

- **Synthetic Multi-Venue Market Data**: Simulates price and volume for assets (BTC, ETH, etc.) across several venues with realistic volatility and volume patterns.
- **TWAP Strategy Implementation**: Slices orders for a given asset and time horizon, and performs simulated executions at nearest available quotes.
- **Performance Analysis**: Calculates average execution price, VWAP benchmark, total traded volume, and cost basis in basis points.
- **Visualization**: Plots execution points against the market price curve for visual inspection.

## Usage

Clone or download the repository. You can run the entire simulation by executing:

```bash
python work_trial_task_namit_shrivastava.py
```
Or, to explore piecewise and see inline plots, open the Jupyter notebook:
```bash
jupyter notebook Work_Trial_Task_Namit_Shrivastava.ipynb
```

The scripts require Python 3.x and a few well-known libraries:
- pandas
- numpy
- matplotlib

Install dependencies as needed via:
```bash
pip install pandas numpy matplotlib
```

## Customization Ideas

- Adjust assets and initial prices in the scripts.
- Try alternate execution strategies by extending the `TWAPStrategy` class.
- Modify market generator parameters to test under different simulated conditions (e.g., more venues, higher/lower volatility).

## Authors and Credit

Created by Namit Shrivastava as part of a work-trial task.

---

For any suggestions or contributions, feel free to fork or submit pull requests!
