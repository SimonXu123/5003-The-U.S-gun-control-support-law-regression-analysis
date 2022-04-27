# Project description
## Project background:

Whether people support gun control or not is always a controversial debate in the United States. On the one hand, people who support gun control often argue that stricter gun control will minimize(减少) gun attacks such as school shootings or terrorist attacks. Those who do not, on the other hand, believe that owning a gun is a basic safeguard against potential dangers such as burglary.

## Project outline

The proposed method is to build serval two-class classification models such as logistic regression, knn, lda and XG-boosting to predict the potential relationship between whether people support gun control and other independent variables.

## Project result:

As the XGBoost achieved the highest F1-score, Kappa and the biggest proportion auc from roc plot, we finally choose it as our optimal classifier to predict people who favor or oppose the gun control law. We also find that black Catholic female non-gun owner with a college degree aged 25-44 who considered herself a Democrat, is more likely to be a supporter of strict gun control

- XGboost model is able to perform a high training calculation with less cost. Due to the high feature dimension of the data set, XGboost can better perform classification prediction through the method of ensemble learning.
- LDA model can improve the accuracy through prior knowledge of the category but is not suit higher requirements for the distribution of data. The data distribution of this data set is relatively stable after data preprocessing and missing and outliers are removed.
- Logistic regression(LR) model performs fast and is easy to apply. As is a linear classifier, it cannot handle the correlation between features. When the feature space is large, the performance is not good. Therefore, the LR model is difficult to fully fit in our dataset, resulting in a very low accuracy rate of the model.
- KNN model is very simple and has a wide range of applications. But the computational cost is very high. Although the accuracy and stability of the model are not much different from the optimal model on this data set. The efficiency of this model is very low.
