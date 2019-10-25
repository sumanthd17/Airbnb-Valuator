The Repo contains the code for Automatic Valuation for Airbnbs

Dataset: New York City Airbnb Open Data

# Models trained

## 1. Random Forest Regressor

```
Random forest is a Supervised Learning algorithm which uses ensemble learning method for classification and regression.
Random forest is a bagging technique and not a boosting technique. The trees in random forests are run in parallel. There is no interaction between these trees while building the trees.
```
### Usage
```
rfr_baseline.predict(X_test)
```

### Results
```
algorithm               | training error | test error
Random Forest Regressor	| 0.037803       | 0.213201
```

## 2. XGBoost Regressor
```
Boosting is an ensemble technique where new models are added to correct the errors made by existing models. Models are added sequentially until no further improvements can be made. In XGBoost, we fit a model on the gradient of loss generated from the previous step. In XGBoost, we just modified our gradient boosting algorithm so that it works with any differentiable loss function.
```
### Usage
```
xgb_baseline.predict(X_test)
```

### Results
```
algorithm    | training error | test error
XGBRegressor | 0.111352       | 0.185248
```
