# Pandas-Challenge-1

<div align='center'>
    <img src='https://images.pexels.com/photos/4483610/pexels-photo-4483610.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1' height='300' title='Inventory stocked on the shelves of a warehouse (image courtesy of Pexels)' alt='An image of a storage warehouse aisle showing the perspective of looking down a series of rows loaded with inventory.'/>

*Wholesale Data Analysis*[^1]

## READ ME
</div>

## Table of contents

* [Overview](#Overview)
* [Execution](#Execution)

---

## Overview

### *The Assignment*

For our Week 4 Challenge we were tasked with completing the provided Jupyter Notebook `wholesale_data_anaysis_starter_code.ipynb` to analyze the information in the provided csv `client_dataset.csv` by exploring, transofrming, confirming, and summarizing the pertinant details relating to both the top clients and their orders. The steps we were charged with completing were:

1. Explore the Data
    * Import the data from the `client_dataset.csv` file into the `wholesale_data_anaysis_starter_code.ipynb`
    * View the column names from the created DataFrame `df`
    * Describe the basic statistics of `df` using the Describe Function
    * Further explore the data
    * Answer the following questions with Pandas;
        * What three item categories had the most entries?
        * Of the category with the most entries, which subcategory had the most entries?
        * Which five (5) clients had the most entries?
            * *These clients' `client_id`s were then to be stored in a List*
        * How many total units did the client with the most entries order?
2. Transform the Data
    * Create a column and calculate the subtoatl of each line
    * Create a column and dynamically calculate shipping prices of each line
    * Create a column and calcuate a total that includes sales tax of each line
    * Create a column and calculate the cost of each line
    * Create a column and calculate the profit of each line
3. Confirm the Work
    * Confirm the calculations for several lines with provided totals
4. Summarize and Analyze
    * Calculate the total prices for the top five (5) clients from the created List
    * Create a summary DataFrame showing the totals for the top five (5) clients with selected information from `df`
    * Sort said data by total profit
    * Format the data in monetary columns into `$X.XXM`
    * Rename the columns in the summary DataFrame for readability
    * Write a few sentences with the summary of our findings

### *Written in*

Jupyter Notebook using Python v3.10.13 and Pandas

### *Accessing the notebook*

To access the wholesale data analysis notebook, simply download the `.ipynb` file `wholesale_data_anaysis_starter_code.ipynb` and the `Resources` folder in this repository into one directory, then load the `wholesale_data_anaysis_starter_code.ipynb` file into Jupyter Notebook through your terminal.

---

## Execution

### *How to use*

Simply `Run All` to execute the code in every cell of the notebook in sequence. Alternatively, each cell may be `Run` on its own, though it is still recommended to run them in order.


[^1]: Image courtesy of free source image site, <a href='https://www.pexels.com/photo/warehouse-with-concrete-floors-4483610/' title='Link to Pexels listing for image'>Pexels</a>