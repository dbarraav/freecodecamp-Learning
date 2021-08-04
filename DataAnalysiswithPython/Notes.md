# Data Analysis with Python
## Pandas Introduction
* Initialize pandas series by usin pd.Series([array], index=[rowname])
* When you print out pandas series/dataframe with specific condition, only those that meet the condition will be printed out. In addition, the datatype(int64) will also be printed out

## Pandas DataFrame
* pd.iloc[[column] gives you rows of column number

## Pandas Conditional Selection and Modigying DataFrames
* pd.index is names of rows. pd.dataframe() is equal to columns

## Pandas Creating Columns
* You can create columns by setting array equal to pd['[column name]']

## Data Cleaning Introduction 
* np.nan
* pd.notnull(), pd.na(), pd.isnull()
* pd.notnull().sum() gives sum of boolean result

## Data Cleaning with DataFrames
* pd.fillna(method='ffill') - propagate last valid observation forward to fill NA

## Data Cleaning Duplicates
* .duplicated() returns boolean series for data frame. A TRUE value is returned when a second occurrence of that value is observed

## Data Cleaning and Visualization
* import matplotlib.pyplot as plt 
* Follow it by %matplotlib inline
* Global API and object-oriented API
    * Global API - using functions at module level.
    * pt.subplot(#,#,#) -> rows, columns, panel selected
    * pt.legend, pt.xlabel, pt.ylabel, pt.plot,
* OOP interface
    * axes start at top left and go row by row
    * plt.scatter, plt.colorbar, pt.figure, pt.hist
    * Combine plots
**GO OVER THIS TUTORIAL AGAIN FOR BETTER UNDERSTANDING**

## Reading Data Introduction
* To import data from csv, first import csv (library)
* Understand "with open() as [val]". Understand opening file, writing to file, reading file, and such

## Reading Data CSV and TXT
* Use pd.read_csv() to read file into dataframe
* There are other functions to read different files with other formats into pandas dataframe
* In addition, there are further arguments that can be added to reading functions 
* Also, there will be a to_csv() to a read_csv. The to_csv allows one to write data to a specific file 

## Reading Data from Databases
* One can import sqlite3 (library) to read from SQLite database
* We use sqlite3.connect() to connect to database
* The .cursor() command create a method "execute" to receive SQL parameters
* The .fetchall() method fetches all results from query, when .execute() was used. 
* One can then use pd.DataFrame to turn it into a dataframe
* Another method is to us pd.read_sql after we use sqlite3.connect()
* .read_sql is shell method for two other methods
    * read_sql_query()
    * read_sql_table()
* To read data from HTML table, first pip install lxml
* One pandas method is .read_html(). This looks for multiple tables

## Parsing HTML and Savind Data
* import requests (library)
* Use val = requests.get([url]), then use val2 = pd.read_html(val.text) to read table
* Indexing val2 gives you specific table
* Read Excel files
    * Use pd.read_excel()
    * Use pd.ExcelFile() - uses ExcelFile class
        * .sheet_names() gives sheet names
        * .parse()
    * Also pd.to_excel() function
    * One can position startrow and starcol arguments in pd.to_excel() function
    * pd.ExcelWriter - write to excel file

## Python Functions and Collections
* Introduction of sets - they are unordered and only contain unique elements.
    * .add(), .pop() -- functions to add value and remove value

## Python Iteration and Modules
* Iterate over key and values with dictionary.items() and for loop
* Remember try and except method

# Numpy
## Initalize Array Problem
* Read more about indexing, where index is negative
    * Understand start and stop index
## Loading Data and Advanced Indexing
* Function to get data from text file is np.genfromtext([filename], [delimiter])
