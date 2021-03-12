# Evaluation_repo
The Implementation of the Evaluation Task for the Atlas Autoencoders Project.
The CSV dataset given is first preprocessed to get a List of all the values corresponding to the Symbol Id 'j' which is the object jet.
Then the Data is converted into a dataframe. 22661 rows x 5 columns

![alt text](https://github.com/bp-high/Evaluation_repo/blob/main/Img1.png)

Then I drop the 'obj' column and convert the values of rest of the column from object to float64 type.

![alt text](https://github.com/bp-high/Evaluation_repo/blob/main/image2.png)

Then I checked if there are any NaN or Inf values present in the Data . As they were no such values present I went on and Normalized the values according to the format they were to be passed on the Autoencoder Network Jupyter notebook.

![alt text](https://github.com/bp-high/Evaluation_repo/blob/main/img3.png)

Then I Split the dataframe into two sets of train and validation set data using 80/20 split as I thought was done with the example files passed to the Autoencoder Network Jupyter notebook. 
After Splitting I pickled both the train and validation sets using protocol version 4 so as to maintain support with Python 3.4+ instead of only Python 3.8 and Python 3.9

![alt text](https://github.com/bp-high/Evaluation_repo/blob/main/image4.png)

In the end I passed the datasets to the Autoencoder Network Jupyter notebook so as to observe the results of the network on the dataset.
