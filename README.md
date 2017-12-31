## Model to improve the Zestimate residual error

Zillow’s Zestimate home valuation has shaken up the U.S. real estate industry since first released 11 years ago.   

“Zestimates” are estimated home values based on 7.5 million statistical and machine learning models that analyze hundreds of data points on each property. And, Zillow has been continually striving to improve the median margin of error from 14% at the onset to 5% today.   

In this project, taken up from the Kaggle competition : "Zillow Prize: Zillow’s Home Value Prediction (Zestimate)" the objective is to improve the Mean Absolute Error between the predicted log error and the actual log error.  

The log error is defined as logerror = log(Zestimate) − log(SalePrice)  

### Why model residual error

The residual errors from forecasts on a time series provide another source of information that we can model.  

More on this [here](https://machinelearningmastery.com/model-residual-errors-correct-time-series-forecasts-python/).

### Data

Zillow provided a full list of real estate properties in three counties (Los Angeles, Orange and Ventura, California) data in 2016-17. Following are these data files and can be accessed [here](https://www.kaggle.com/c/zillow-prize-1/data) :  
- properties_2016.csv - all the properties with their home features for 2016.  
- properties_2017.csv - all the properties with their home features for 2017.  
- train_2016.csv - the training set with transactions from 1/1/2016 to 12/31/2016.  
- train_2017.csv - the training set with transactions from 1/1/2017 to 9/15/2017.  

Each Input sample represents a real estate property. A real estate property can be a residential house, commercial setting or even an empty land.   
Following are some examples of the features of an input sample:  
- Total area (finished or unfinished) of the property  
- Total assessed value of the property  
- Neighborhood,region, city, zip, state of the property  
- Property Zoning code assigned by a municipal authority  
- Kind of material used to build the house if applicable  
- Total number of bathrooms, bedrooms, pools, patios, spas, garages, floors,fireplaces etc. on the property if applicable   

The output or target variable is an error value called logerror that represents the difference between the log (Zestimate) and log (Actual Sales Price). Zestimate is the Zillow’s prediction of the monetary value of that property while actual sales price is the price at which that property actually got sold.  

### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [xgboost](http://xgboost.readthedocs.io/en/latest/)  
- [seaborn](https://seaborn.pydata.org/)  
- [ggplot](http://ggplot.yhathq.com/)  
- [NumPy](http://www.numpy.org/)  
- [Pandas](http://pandas.pydata.org)  
- [matplotlib](http://matplotlib.org/)  
- [scikit-learn](http://scikit-learn.org/stable/)  

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed, you can install the same from [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included.

### Code

Main code is provided in the `customer_segments.ipynb` notebook file. You will also be required to use the included `visuals.py` Python file and the `customers.csv` dataset file to complete your work. If you are interested in how the visualizations are created in the notebook, please feel free to explore the code included in `visuals.py`.

### Run

In a terminal or command window, navigate to the top-level project directory `customer_segments/` (that contains this README) and run one of the following commands:

```bash
ipython notebook customer_segments.ipynb
```  
or
```bash
jupyter notebook customer_segments.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.
