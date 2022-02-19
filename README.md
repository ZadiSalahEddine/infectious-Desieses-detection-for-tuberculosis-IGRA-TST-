The "interferon.csv" is the original DataSet that contains informations about the IGRA test and TST for tuberculosis infection. the attributes are just some blood sample components, but  the DataSet contains a lot of missing values.
to Handle-missing-values using Feature-engineering techniques i used online "CSV to SQL" converter, then i used Oracle SQL Developer to change all  the datatype that are String to Number because Categorical data can take values like numbers by that we can treat them the same and then we can do the math on it.
How to do the Math 
there are 3 options to handle missing data:
1- delete the row if it does not effect the accuracy of the ML model and it has no gain. 
2-create a ML model to predict the missing value (boring and takes time and you have to get paid for that lol)
3-use statistical techniques (mean, median, mode of) sounds great for me

to apply the 3rd option you have to bare in mind that you will get duplicated values, so for that we have to set a range and add a random number to the ((mean, median, mode of)) with respect to every selected features for further steps.

   Now we have the 'interferon1_UPDATED.csv' it's a prepare datset ready to  get visualize, analyzed and ready to make ML model train and test
