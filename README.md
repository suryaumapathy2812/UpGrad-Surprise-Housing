# Surprise Housing

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below. 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.


### The company wants to know:
- Which variables are significant in predicting the price of a house
- How well those variables describe the price of a house.

 Also, determine the optimal value of lambda for ridge and lasso regression.

### Business Goal  

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.


## Conclusion

We obtained satisfactory performance scores for both Ridge and Lasso regression models:

- **Ridge Regression:**

  - Training score: 90.9
  - Testing score: 87.4

- **Lasso Regression:**
  - Training score: 89.8
  - Testing score: 86.4

### Top 5 Most Significant Variables

The most significant variables identified by the models are as follows:

#### Ridge Regression:

1. **SaleCondition_Partial**: 0.143
2. **SaleCondition_Others**: 0.105
3. **SaleCondition_Normal**: 0.099
4. **GarageFinish_Unf**: 0.094
5. **GarageFinish_RFn**: 0.092

#### Lasso Regression:

1. **SaleCondition_Partial**: 0.198
2. **SaleCondition_Others**: 0.12
3. **SaleCondition_Normal**: 0.098
4. **GarageFinish_Unf**: 0.084
5. **GarageFinish_RFn**: 0.079

### Interpretation

These variables indicate significant contributions to predicting house prices, with higher coefficients reflecting greater impact. For example, houses with the "SaleCondition_Partial" feature are highly influential in both models.

### Optimal Lambda Values

- **Ridge Regression:** The optimal value of lambda (regularization parameter) is 10.
- **Lasso Regression:** The optimal value of lambda is 0.001.

### Model Choice

Given the feature selection capabilities of Lasso regression, where it effectively shrinks some coefficients to zero, making it easier to interpret which features are most important, Lasso regression may be the preferred choice for this case. This feature selection can be particularly beneficial in reducing model complexity and enhancing interpretability.

### Summary

Both Ridge and Lasso regression models provide valuable insights and strong predictive performance. However, due to its feature selection properties, Lasso regression might be more advantageous for this particular dataset and problem context.
