# Final Project

In this final project, you will convert a convert notebook style code for comparing different
tabular data prediction tasks into a shareable
BenchOpt benchmark --- you will then extend the benchmark with more methods, datasets, and 
control parameters.

## Prerequisites

This homeworks assumes you already possess a github account. It also assumes you have `git`, `pip`, and `conda` 
installed on your computer. If not, there are many resources online for installing them: Please 
independently install them using the resource of your choice before proceeding.

## Setup

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

## Getting Started With BenchOpt

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


