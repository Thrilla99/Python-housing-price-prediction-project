# Python-housing-price-prediction-project
The goal of this project is to predict house prices based on features such as square footage, number of bedrooms/bathrooms, location, and other housing attributes.

House Price Prediction – Summary

In this project, I explored different regression approaches on the King County housing dataset to predict house prices.

Simple Linear Regression (1 feature): R² ≈ 0.49 — baseline performance.

Multiple Linear Regression (many features): R² ≈ 0.65 — improved accuracy with more predictors.
Pipelin wiht polynomial- 0.75

Ridge Regression: R² ≈ 0.68 — stabilized coefficients in the presence of multicollinearity.

Polynomial Features + Ridge: R² ≈ 0.59 — captured some non-linear effects but introduced numerical challenges (ill-conditioned matrix).

Takeaway:
Each modeling step added complexity, but the best trade-off in this dataset came from multiple regression with ridge regularization. Polynomial expansion showed the challenges of handling high-dimensional feature spaces, a valuable lesson for future projects.


## Final Conclusions  

### Baseline Model (Linear Regression with one feature)  
- Established a simple baseline for prediction.  
- Useful for understanding relationships but limited in accuracy.  

### Multiple Linear Regression  
- Adding more features improved the explanatory power of the model.  
- Highlighted how additional predictors can reduce bias but may introduce collinearity.  

### Ridge Regression  
- Applied to handle multicollinearity and stabilize coefficients.  
- Achieved better generalization compared to the plain linear regression.  

### Polynomial Features + Ridge  
- Explored non-linear relationships by expanding features.  
- The model ran successfully, but prod
uced a warning about an *ill-conditioned matrix*, which indicates that polynomial transformations can create highly correlated features.  
- Ridge regularization helped mitigate this, but performance gains were modest, and computation became more resource-intensive.  

---

## Key Takeaways From Final Conclusions  
- Linear regression is easy to interpret but limited in predictive power.  
- Ridge regression improves stability when features are correlated.  
- Polynomial features add flexibility but can introduce serious computational and numerical challenges.  
- In practice, careful feature selection and preprocessing are necessary before applying polynomial expansions at scale.  
