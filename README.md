## Model to improve the Zestimate residual error

Zillow’s Zestimate home valuation has shaken up the U.S. real estate industry since first released 11 years ago.   

“Zestimates” are estimated home values based on 7.5 million statistical and machine learning models that analyze hundreds of data points on each property. And, Zillow has been continually striving to improve the median margin of error from 14% at the onset to 5% today.   

In this project, taken up from the Kaggle competition : "Zillow Prize: Zillow’s Home Value Prediction (Zestimate)" the objective is to improve the Mean Absolute Error between the predicted log error and the actual log error.  

The log error is defined as logerror = log(Zestimate) − log(SalePrice)  

### Data

Zillow provided a full list of real estate properties in three counties (Los Angeles, Orange and Ventura, California) data in 2016-17. Following are these data files and can be accessed [here](https://www.kaggle.com/c/zillow-prize-1/data) :  
properties_2016.csv - all the properties with their home features for 2016. 
properties_2017.csv - all the properties with their home features for 2017 
train_2016.csv - the training set with transactions from 1/1/2016 to 12/31/2016
train_2017.csv - the training set with transactions from 1/1/2017 to 9/15/2017 

### Contribution Guidelines

Here are the important ways you can contribute:

by coming up with a model that further reduces the error.  
by writing or editing documentation
by adding comments and clean up inconsistent whitespace 

### Submitting a Pull Request

Fork the official repository.
Create a topic branch.
Implement your fix.
Add, commit, and push your changes.
Submit a pull request.

### Notes

Please add tests if you changed code.  
Contributions without tests won't be accepted.
