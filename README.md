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

### *Breaking down the cells*

Below is a more in-depth explanation of the various cells coded within the `wholesale_data_anaysis_starter_code.ipynb` notbook.

| Cell (in order from top to bottom) | Notes[^2] (on the contained code) |
| ---: | :--- |
| *Markdown 1* | *Explanation for the purpose of cells 1 through 9* |
| *1* | *Importing Pandas and the `client_dataset.csv` file, then adding the data from the `client_dataset.csv` file to the DataFrame `df`* |
| 2 | Viewing the column namess for `df` |
| 3 | Gathering the basic statistics for `df` |
| 4 | A cell for additional research (various lines of code tested and commented out durring development, retained to demonstrate purpose of cell) |
| 5 | Calculating what categories had the most entries in `df` (stored in variable `top3_cats`) |
| 6 | Calculating what subgategory had the most entries from the category with the most entries in **Cell 5** (stored in variable `top_cat_top_subcat`) |
| 7 | Calculating the top five (5) clients by entry ammounts in `df` (stored in variable `top5_clients`) |
| 8 | Converting `top5_clients` to the list `top5_clients_list` for later use |
| 9 | Calculating how many units the client with the most entries in `df` ordered (stored in variable `top_client_tot_units`) |
| *Markdown 2* | *Explanation for the purpose of cells 10 through 19* |
| 10 | Declaring `line_subtot` to calculate the subtotal for a given line of `df`, then creating the test DF `subtot_confirm` to confirm the line subtotal is calculated correctly |
| 11 | With `line_subtot` confirmed, creating the working DF `df_totals`[^3] for future data manipulation and creating a column for `line_subtotal` (copied from `df`, and ensures the original data is preserved) |
| 12 | Declaring `tot_weight` to calculate the total weight for a given line of `df_totals`, defining `calc_ship_price` tp apply a shipping price based off the calculated total weight, and then creating the test DF `shipping_confrim` to confirm the total weight and shipping price are calculated correctly |
| 13 | With `tot_weight` and `calc_ship_price` confirmed, adding columns `total_weight` and `shipping_price` to `df_totals` with the calculated values |
| 14 | Declaring `line_price` to calculate the total price for a given line of `df_totals`, then creating the test DF `line_price_confirm` to confirm the line price is calculated correctly |
| 15 | With `line_price` confirmed, adding column `line_price` to `df_totals` with the calculated values |
| 16 | Declaring `line_cost` to calculate the total cost for a given line of `df_totals`, then creating the test DF `line_cost_confirm` to confirm the line cost is calculated correctly |
| 17 | With `line_cost` confirmed, adding column `line_cost` to `df_totals` with the calculated values |
| 18 | Declaring `line_profit` to calculate the total profit of a given line of `df_totals`, then creating the test DF `line_const_confirm` to confirm the total profit is calculated correctly |
| 19 | With `line_profit` confirmed, adding column `line_profit` to `df_totals` with the calculated values |
| *Markdown 3* | *Providing order id's and totals to confirm calculations match reciepts* |
| 20 | Declaring `order_A_tot`, `order_B_tot`, and `order_C_tot` to sume the `line_price` for all records matching the provided `order_id`s, then printing the results in formatted strings |
| *Markdown 4* | *Explanation for the purpose of cells 21 through 24* |
| 21 | X |
| 22 | X |
| 23 | X |
| 24 | X |
| Markdown 5 | X |

[^1]: Image courtesy of free source image site, <a href='https://www.pexels.com/photo/warehouse-with-concrete-floors-4483610/' title='Link to Pexels listing for image'>Pexels</a>

[^2]: Cells with provided code will be italiziced.

[^3]: All future manipulation of data will ultimately be based off `df_totals` from cell 11 and onwards, unless otherwise noted.