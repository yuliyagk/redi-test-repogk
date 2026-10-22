## Data Analysis and Time Series Forecasting with Python

This repository contains learning notebooks exploring tabular data analysis, numerical computation and seasonal time series forecasting.

The exercises use Pandas and NumPy for data exploration and statsmodels for energy load forecasting.

## Project Overview

The goal of these notebooks is to:

* Explore datasets using Pandas
* Inspect categories and missing values
* Practice filtering, aggregation and duplicate removal
* Perform matrix operations with NumPy
* Visualize energy consumption over time
* Build seasonal ARIMA models
* Generate rolling forecasts

## Tech Stack

* Python
* Pandas & NumPy
* Matplotlib
* Scikit-learn
* Statsmodels
* Jupyter Notebook / Google Colab

## Notebooks

### 1. Data Analysis and NumPy Exercises

File: `HAMLBootcamp.ipynb`

This notebook uses a car dataset to practice:

* Inspecting dataset structure
* Counting records by manufacturer
* Finding unique car models
* Identifying missing values
* Exploring median and mode
* Removing duplicate feature combinations
* Calculating linear regression weights using matrix operations

The saved outputs show a dataset with 11,914 rows and 16 columns.

### 2. Seasonal Time Series Forecasting

File: `ARIMA.ipynb`

This notebook explores hourly energy load data and includes:

* Time series visualization
* Chronological train/test splitting
* MinMax scaling fitted on the training data
* Seasonal ARIMA modeling through SARIMAX
* A daily seasonal period of 24 hours
* Rolling forecasts with a 720-hour training window
* Three-step forecast generation

The saved outputs include fitted model summaries and forecast values.

## Workflow

Data → Exploration → Preparation → Visualization → Numerical Analysis / Seasonal Modeling → Predictions

## How to Run

### 1. Install dependencies

```bash
pip install pandas numpy matplotlib scikit-learn statsmodels jupyter
```

The original notebooks were created with older package versions. Dependency adjustments may be needed.

### 2. Open the notebooks

```bash
jupyter notebook
```

Choose:

* `HAMLBootcamp.ipynb` for tabular data analysis and matrix exercises
* `ARIMA.ipynb` for seasonal forecasting

### 3. Prepare the data

The car-data notebook downloads its dataset directly from the ML Bookcamp repository.

The forecasting notebook expects:

* Energy data in a local `data/` directory
* A `common.utils` module providing `load_data` and `mape`

These supporting files are not included in this repository. Obtain the corresponding materials from the Microsoft ML for Beginners time series lessons before running the forecasting notebook.

## Project Status

* This repository is a collection of educational exercises.
* Saved notebook outputs illustrate the original analysis and modeling work.
* The forecasting notebook requires additional data and helper files.
* The final forecast-evaluation cell needs correction before reporting forecast metrics.
* The missing-value exercise should use a scalar mode value to fill all missing Engine HP entries.
* Execution with current dependencies has not been verified.

## Use Cases

* Practicing exploratory data analysis
* Understanding missing data and categorical summaries
* Learning the matrix formulation of linear regression
* Exploring seasonality in energy consumption
* Practicing rolling time series forecasting

## Learning Outcomes

Through these exercises I practiced:

* Inspecting and filtering data with Pandas
* Working with missing values and duplicate records
* Performing matrix calculations with NumPy
* Visualizing time-dependent data
* Separating training and test periods chronologically
* Scaling data without fitting on the test set
* Fitting seasonal statistical models
* Implementing a rolling forecasting workflow

## Acknowledgments

The car-data exercises use materials and data from DataTalksClub's Machine Learning Zoomcamp and ML Bookcamp:

https://github.com/DataTalksClub/machine-learning-zoomcamp

https://github.com/alexeygrigorev/mlbookcamp-code

The forecasting notebook references Microsoft ML for Beginners:

https://github.com/microsoft/ML-For-Beginners/tree/main/7-TimeSeries
