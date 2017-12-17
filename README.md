### Build a model to improve the Zestimate residual error

Zillow’s Zestimate home valuation has shaken up the U.S. real estate industry since first released 11 years ago.   

“Zestimates” are estimated home values based on 7.5 million statistical and machine learning models that analyze hundreds of data points on each property. And, Zillow has been continually striving to improve the median margin of error from 14% at the onset to 5% today.   

In this project, taken up from the Kaggle competition : "Zillow Prize: Zillow’s Home Value Prediction (Zestimate)" the objective is to improve the Mean Absolute Error between the predicted log error and the actual log error.  

The log error is defined as logerror = log(Zestimate) − log(SalePrice)
