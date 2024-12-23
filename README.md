Machine Learning - Data Processing 

Upload the two files to Google Collab 

****Run commands ********

import pandas as pd  > converts data into a table 
import numpy as np 

pd.read_csv() - to import data 

=======================================================

sslc = pd.read_csv('marks.txt', sep = ';', header= None , index_col = None)

sslc.columns = ['region', 'roll_number' , 'fl','sl','math','sci','ss','total','pass','withheld','extra']

sslc['fl'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['sl'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['math'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['sci'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['ss'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['total'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

=====================================================

****Functions to run****


.head() - shows first 5 rows 
.tail() - shows last 5 rows 
.size - returns no of data(cells) in the data frame 
.count() - returns the number of non-null value in each column 
.shape - how many rows and how many columns > tuple 
.ndim - returns the number of dimentions: two , three ... etc 
.info 
.nunique() - how many unique values in each column 
.describe() - showing statistical methods like count / mean / standard deviation / min / 25% / 50% / 75% / max 
  .describe(include =[]) - add data type like object / int / float / all 
  .describe(exclude =[])

.memory_usage() 
.columns
sslc['column name'] - access a specific column 
.iloc[0] - select row 
.set_index() set a custom index 
.loc[] - select row 
.isnull().sum() 
.unique() - returns all unique values in the selected column 
.replace()

