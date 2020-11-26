My work is in Google Collaboratory
https://colab.research.google.com/drive/1xUSKhyM5i_DmnLuKnRTPn1IfQLqezwV-

good work can be found here... you can also update the code and try it out
https://research.google.com/seedbank

## Steps in Data Exploration (EDA: Exploratory Data Analysis)
1. ### df.describe()
- normal distribution of data is preferred
- Std Deviation - should be a small fraction of the mean... eg: if 6ft is the mean height, std dv of 3-4 inches is good... if sd is 3 ft... data does not make sense SD of 3 inches mean, 68% of the population are in the range of 5'9" and 6'3"
- if the diff between mean and median is too large... data will be skewed
- if data distribution curve is too narrow or too wide, it is not following the normal bell curve distribution.. and the data point may not be very helpful


1. ### seaborn.pairplot & df.corr() 
- will tell me, which dimentions has a co-relation to the dimentaion we are interested in... in pairplot, if it is all over the place with no relation... that data point may not help us... however, if the datapoints are going up... or down with the x-axis... then there either is a positive or a negaitve co-relationship... in df.corr() a feature that has a co-rel of a number closer to -1 or +1 is preferred.... numbers closer to 0 won't help much


1. ### heatmap sns.heatmap(df.corr(), annot=True)
- Will hilight the co-relations closer to -1 or +1
