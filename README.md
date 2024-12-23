Machine Learning - Data Processing 

Upload the two files to Google Collab 

Run commands gmail


sslc = pd.read_csv('marks.txt', sep = ';', header= None , index_col = None)

sslc.columns = ['region', 'roll_number' , 'fl','sl','math','sci','ss','total','pass','withheld','extra']

sslc['fl'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['sl'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['math'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['sci'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['ss'] = pd.to_numeric(sslc['fl'], errors = 'coerce')

sslc['total'] = pd.to_numeric(sslc['fl'], errors = 'coerce')
