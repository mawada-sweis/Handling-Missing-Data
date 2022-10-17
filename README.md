# Handling Missing Data in Python

I have to analyze a relatively large amount of data and get rid of all the missing values in the dataset. The challenge in this assignment is to apply the various methods on more than 45000 observations and more than 200 features.

At the first, I deleted columns that were missing data more than 65% of the data of the column and eliminated rows when more than half of the row is missing.
After this step, I have a shape(43084, 165).

The data was then divided into two types (numerical and categorical) because the methods for dealing with each differed.
  - The numarical data handled by the mean statistic method for each column. (Because I could not detect a distinction between the data, I did not think there was a need to apply more than one method to deal with missing data.)
  - The categorical data handled by 2 method: 
    - Using farward/back fill method for columns, the values around the missing data may be more accurate.
    - Using most frequent value of column method for Columns, in my opinion, do not rely on the data around them.

Finally, I merged the category and numerical data to create a final dataframe with no missing data.
