Will it Rain?

Data sourced from : https://www.kaggle.com/jsphyg/weather-dataset-rattle-package

#### Binary classification implemented with logistic regression which uses meteorological data to predict wheather it will rain.


### How it works:

- Choose feature to use and input feature keys from list below into list: 'input_features'. This must also include 'RainTomorrow' key. 
- Input measurements of these featuers in the same order as the key names in 'input_features' into list: 'value_input'.
- Input full meteorological data set. 

Features Options: 

MinTemp           
MaxTemp            
Rainfall          
Evaporation      
Sunshine            
WindGustSpeed           
WindSpeed9am      
WindSpeed3pm      
Humidity9am       
Humidity3pm       
Pressure9am      
Pressure3pm      
Cloud9am         
Cloud3pm         
Temp9am            
Temp3pm      

### When it runs it will:

- Clean the selected feature columns of NaN values.
- Calculate number of data points, and size of test and training sets.
- Shuffle the data to eliminate original time ordering and divide into training and test sets.
- Rescale all features. 
- Run gradient descent to train logistic regression algorithm.
- Plot cost function history to ensure convergence.

### It will output:

- Accuracy of training and test set predictions.
- Confusion matrix with percentages of True Positive, True Negative, False Positive and False Negative preditions.
- Predition of 'it will rain' or 'it will not rain' for given input measurements in list 'value_input' (with sigmoid value, i.e. where along the sigmoid does this prediction fall). 