# SC1015 Data Science Project

## Problem Definition

Given this ["Key Indicators of Heart Disease" dataset](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease), which has many various indicators, we want to build a model that can use these indicators, that any regular adult can obtain through a health screening, to evaluate the risk that any given individual has for heart disease.

##

## Conclusion

- We are able to evaluate risk of a given individual with reasonable accuracy.
- Through EDA and feature selection, we found out that while there are many features, only a few of them proved to have more significance at predicting if an individual had a heart attack

## Learning Outcomes

- Importance of reproducible notebooks
  - Working asynchronously, it is best to reproducible code, so that other group mates can replicate the results. Often, it is easy to write "throwaway" code in notebooks, and other group members are not able to reproduce it.
- Handling a massively imbalanced dataset (1:24, minority : majority)
  - Undersampling can help balance the classes while maintaining the integrity of the information. It allows for better exploratory data visualisation to try and spot features with some form of correlation.
  - However, in our case, undersampling removed too many data points which hurt our model's ability to perform.
  - Thus, we learnt to resample the dataset with both oversampling and undersampling methods.
- New machine learning models
  - Logistical regression
  - Random forest
- Cross Validation
  - Sometimes, test accuracy itself is not accurate enough. If the dataset is small enough (perhaps in the case of an undersampled dataset), it is possible that the shuffle might not be big enough and the test accuracy is not representative.
  - To fix this, when we evaluate our models, we do cross validation. This evaluates the model $n$ times and lets us avoid this problem of wondering if the test accuracy is good enough. This will give us a more accurate measure of how well a model is performing.
- Feature selection
  - When there are many features, we want to be able to find out which features are good. There are many methods to evaluate a predictor's significance to response to variable.
  - In this case, we used the `chi2` feature selector as majority of our features are categorical with few numerical
  - It is also important to not just take the feature selected values at face value and consider more or less features and test it out in practice. In our case, we found that the top 5 features were the most impactful.
- Suitable metrics to target problem
  - Given the medical nature of this problem, the Recall metric of the model's performance is more critical as it could be a problem if our model has high accuracy with low true positive (heart attack).

## Individual Contributions

- Chua Ze Ming, [lczm](https://github.com/lczm)
- Nick Lee, [Nicklee4](https://github.com/Nicklee4)
- Madhav, [Madhav-byte-debug](https://github.com/Madhav-byte-debug)

## References

- https://medium.com/@Kavya2099/optimizing-performance-selectkbest-for-efficient-feature-selection-in-machine-learning-3b635905ed48#:~:text=SelectKBest%20uses%20statistical%20tests%20like,in%20the%20final%20feature%20subset.
- https://medium.com/data-science-at-microsoft/five-mistakes-to-avoid-when-modeling-with-imbalanced-datasets-d58a8c09929c#:~:text=Resampling%20the%20validation%20and%20test,leakage%20in%20your%20evaluation%20setups.
