<h1 align="center">Introducing Pandas</h1>


# Introduction:
Pandas is an open-source Python library widely used for data manipulation and analysis.It was invented by Wes McKinney in 2008.It is used for working with data sets.It allows us to analyze big data and make conclusions based on statistical theories.It can clean messy data sets, and make them readable and relevant.Pandas is built around data structures called Series and DataFrames.

# Installation Process :
pip install pandas

# Importing :
Pandas are customarily imported as pd. 

Example:

  import pandas as pd

# Data structures:
# Pandas primarily relies on two data structures:

# 1.Series:

A one-dimensional labeled array capable of holding any data type. It can be thought of as a single column of data.

Example: 
    
s = pd.Series([1, 3, 5, np.nan, 6, 8])
  
  print(s)

# 2.DataFrame:

A two-dimensional labeled data structure with columns of potentially different types. It is similar to a spreadsheet or SQL table, consisting of rows and columns.

Example :

  data = {'col1': [1, 2, 3], 'col2': ['A', 'B', 'C']}
  
  df = pd.DataFrame(data)
   
   print(df)

# Key Functionalities:
Data Loading and Saving:

Pandas can read and write data from various formats, including CSV, Excel, JSON, SQL databases.

Example :
   
   df = pd.read_csv('data.csv')
  
   df.to_excel('output.xlsx', index=False)

# Data Inspection: 
Methods like head(), tail(), info(), and describe() provide quick overviews of the DataFrame's structure, data types, and basic statistics.

# Data Selection and Filtering: 
Data can be selected by column name, row index, or through boolean indexing to filter based on conditions.

Example :
     
   print(df['col1'])               # Select a column
 
   print(df[df['col1'] > 1])     # Filter rows

# Data Cleaning and Transformation: 
Pandas offers tools for handling missing values fillna(), dropna(), renaming columns, changing data types, and applying functions to columns or rows.

# Data Aggregation and Grouping: 
Operations like groupby() enable grouping data by specific criteria and performing aggregations sum, mean, count on the grouped data.

# Merging and Joining: 
DataFrames can be combined using merge() or join() based on common keys or indices, similar to SQL joins.

# Summary :
Pandas is a foundational Python library for data manipulation and analysis, widely used in data science and related fields. It provides powerful and flexible data structures designed to make working with labeled or relational data intuitive and efficient.
