# Tabular-text-file
A group of text files were cleaned and stop words removed using the Linux platform. After which I used Python to create a tabular format of the File name, words and frequency of words. 


import pandas as pd
import numpy as np

f_open  = open('Desktop/Allfiles.txt', 'r')
data = f_open.read()
f_open.close()
print (data)


import pandas as pd
data_array = np.array(data)
print(data_array)


import numpy as np
import pandas as pd

df = pd.read_table('Desktop/Allfiles.txt', delim_whitespace=True, names=('A', 'B', 'C'))
print (df)

f_open  = open('Desktop/masterfile.txt', 'r')
sample = f_open.read()
f_open.close()
print (sample)

import numpy as np
import pandas as pd

df = pd.read_table('Desktop/masterfile.txt',sep = ":" , names=('Title', 'Word', 'C'))
print (df)


