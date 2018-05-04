# Session-3---Logistic-Regression-Revisited
Reviewing Logistic regression and some important concepts.  

This is a reformatted and restructured version of the Iris Data Logistic Regression discussed in Session 2 - only here we focus on each key step and then add regularisation.

The accompanying slides can be seen [here](https://drive.google.com/open?id=173YSJmNomYBjWIlhXJq6-QILDwSEPDZf).


## Things to try
Try changing the test:train split ratio
Experiment with the regularisation parameter (via the Logistic Regression C paramter) and see what it does to the model weights, accuracy and decision boundaries. 


## Information from discussions in the session
The sckit-utilities.py package is a small piece of code that we have written to plot the fitted model in 2D and show the decision boundaries. I forgot to include it in this repo initially (SORRY!!) but I have now uploaded it. Just make sure it is in the same directory as the Jupyter notebook and Jupyter will see it and load it. 

Once trained the model produces a set of parameters that fit or model the data. These can be used to make a prediction on new data - either using the trained SciKit-Learn object or within your own function and code. You can see the paramters the model has learnt from your data by calling the ```get_params``` method.

```python
lr.get_params()
```

The Logistic Regression Documentation can be found [here](http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) 

We were also asked about teh difference between cost, error and loss functions. Well it seems it varies on people and definitions but there is a decent explanation in [here](https://www.quora.com/What-is-the-difference-between-a-cost-function-and-a-loss-function-in-machine-learning). A loss function tends to describe the error for single training point, while cost function is often defined for the whole training set. 
