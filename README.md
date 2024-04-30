# README.md

# Top and Flop CAC 40 Interactive Visualization

This Python script provides an interactive visualization of the top and flop performers in the CAC 40 index over a user-defined time range. The code uses pandas for data handling, matplotlib for plotting, and ipywidgets for creating interactive controls.

## Requirements

- pandas
- matplotlib
- ipywidgets

## Class: top_n_flop

The `top_n_flop` class takes historical CAC 40 data as input and provides methods to plot top and flop performers over a specified time range.

### Methods

- `__init__(self, history)`: Initializes the class with historical data and sets up a dictionary of time ranges.
- `plot(self, range, n_stock)`: Plots the top and flop performers for the given time range and number of stocks.
- `show(self)`: Displays interactive controls for selecting the time range and number of stocks.

## Usage

1. Import the required libraries and the `top_n_flop` class.
2. Load the historical CAC 40 data into a pandas DataFrame.
3. Create an instance of the `top_n_flop` class with the historical data.
4. Call the `show` method to display the interactive controls and generate the plot.

## Example

```python
# Load historical CAC 40 data into a DataFrame (e.g., from a CSV file)
history = pd.read_csv('cac40_history.csv', index_col='Date', parse_dates=True)

# Create an instance of the top_n_flop class
tnf = top_n_flop(history)

# Display interactive controls and plot
tnf.show()
```
