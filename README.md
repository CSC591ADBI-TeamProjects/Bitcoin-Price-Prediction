# Bitcoin-Price-Prediction
Implement the Bayesian Regression model to predict the future price
variation of bitcoin by following the methogology [1][2] as:

1. Compute the price variations (Δp 1 , Δp 2 , and Δp 3 ) for train2 using train1 as input to the Bayesian Regression equation (Equations 6). Make sure to use the similarity metric
(Equation 9) in place of the Euclidean distance in Bayesian Regression (Equation 6).
2. Compute the linear regression parameters (w 0 , w 1 , w 2 , w 3 ) by finding the best linear fit (Equation 8). Here you will need to use the ols function of statsmodels.formula.api. Your
model should be fit using Δp 1 , Δp 2 , and Δp 3 as the covariates. Note: the bitcoin order book data was not available, so you do not have to worry about the rw 4 term.
3. Use the linear regression model computed in Step 2 and Bayesian Regression estimates, to predict the price variations for the test dataset. Bayesian Regression estimates for test
dataset are computed in the same way as they are computed for train2 dataset – using train1 as an input.
4. Once the price variations are predicted, compute the mean squared error (MSE) for the test dataset (the test dataset has 50 vectors => 50 predictions).


References:<br/>
[1] Shah, Devavrat, and Kang Zhang. "Bayesian regression and Bitcoin." Communication, Control, and Computing (Allerton), 2014 52nd Annual Allerton Conference on. IEEE, 2014.<br/>
[2] The project is part of the coursework 'Algorithms for Data Guided Business Intelligence' by Dr. Nagiza Samatova.
