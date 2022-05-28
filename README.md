# Deep Learning: Charity Funding Predictor

### Background
From Alphabet Soup’s business team, we have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:
* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special consideration for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

### Preprocess the data
We’ll need to preprocess the dataset in order to compile.
Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:

What variable(s) are considered the target(s) for your model?,
What variable(s) are considered the feature(s) for your model?

Drop the EIN and NAME columns.
Determine the number of unique values for each column.
For those columns that have more than 10 unique values, determine the number of data points for each unique value.
Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.
Use pd.get_dummies() to encode categorical variables.

### Compile, Train, and Evaluate the Model
Using TensorFlow, We’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset.  We’ll compile, train, and evaluate our binary classification model to calculate the model’s loss and accuracy.

* Evaluate the model using the test data to determine the loss and accuracy.
* Save and export results to an HDF5 file, and name it AlphabetSoupCharity_moldel.h5.

