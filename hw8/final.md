# Final Project

In this final project, you will convert a convert notebook style code for comparing different
tabular data prediction tasks into a shareable
BenchOpt benchmark --- you will then extend the benchmark with more methods, datasets, and 
control parameters.

## Prerequisites

This homeworks assumes you already possess a github account. It also assumes you have `git`, `pip`, and `conda` 
installed on your computer. If not, there are many resources online for installing them: Please 
independently install them using the resource of your choice before proceeding.

## Read Notebook

1. Go to [https://github.com/xyhan-github/STATS335_F23/blob/master/hw8/TabularDemo.ipynb](https://github.com/xyhan-github/STATS335_F23/blob/master/hw8/TabularDemo.ipynb).

    ####
    
    This notebook contains a simplified version of the code from hw7 that does the following:
    * Loads example tabular datasets from Huggingface:
      * Adult Income: Binary Classification
      * Housing Prices: Regression
      * Forest Covertype: Multi-Class Classification
    * Cleans the data and identifies the type of problem it is.
    * Trains a model Linear, XGBoost, or LightGBM on the data.
   
2. Click the "Open in Colab" button.

3. In Google Colab, read and run the code in the notebook to make sure you understand what it does.

## Setup BenchOpt

1. Open a terminal window on your computer.

3. Install BenchOpt on your computer by typing the following into terminal.
   ```
   $ pip install -U benchopt
   ```

2. Navigate to a directory where you want to store your BenchOpt benchmarks.
   ####
   (In the terminal, you can navigate to a directory by typing `cd <directory path>`.)

3. In terminal, clone the BenchOpt benchmark template into the folder and navigate into it.
   ```
   $ git clone https://github.com/xyhan-github/stats-335_tabular_data
   $ cd stats-335_tabular_data
   ```
   
4. In terminal, install the benchopt dependencies by running
    ```
    $ benchopt install
    ```

5. In terminal, run the template benchmark by running
    ```
    $ benchopt run
    ```
    If everything was set up correctly, this should generate a .html file of results
    that contains the results of running the housing prices and adult income datasets
    on the linear classification model (regression or logistic regression depending on the dataset)
    across three parameter setting for the $L_2$ regularization parameter (`reg_lambda`).
   
## Task 1: Finish adapting the notebook

1. Study the `objective.py`, `solvers/linear_l2.py`, and `datasets/datasets_huggingface.py` files.
2. Using the BenchOpt documentation

   [https://benchopt.github.io/tutorials/build_benchmark.html](https://benchopt.github.io/tutorials/build_benchmark.html)

   get a sense for how the benchmark was adapted from the parts of notebook you read earlier.

3. The notebook is only partially adapted: The benchmark is missing the following:
   * The Forest Covertype dataset
   * The XGBoost and LightGBM solvers
   
   Add these to the benchmark by using the notebook and existing files as a guide.

4. **Submit:** Perform `benchopt run` again. Submit the resulting .html file to Canvas.


