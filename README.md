# SC1015 Data Science Project

## Problem Definition

Given this ["Key Indicators of Heart Disease" dataset](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease), which has many various indicators, we want to build a model that can use these indicators, that any regular adult can obtain through a health screening, to evaluate the risk that any given individual has for heart disease.

##

## Conclusion

- We are able to evaluate risk of a given individual with reasonable accuracy.
- Through EDA and feature selection, we found out that while there are many rows, only a few of them contribute the most when evaluating risk

## Learning Outcomes

- Importance of reproducible notebooks
  - Working asynchronously, it is best to reproducible code, so that other group mates can replicate the results. Often, it is easy to write "throwaway" code in notebooks, and other group members are not able to reproduce it.
- Handling a massively imbalanced dataset (1:24, minority : majority)
  - Undersampling can remove key features. We cannot just look at how many rows exist for the minority class. In this case, we lost a lot of features through undersampling.
  - We learnt to resample the dataset with both oversampling and undersampling methods.
- Cross Validation
  - Sometimes, test accuracy itself is not accurate enough. If the dataset is small enough (perhaps in the case of an undersampled dataset), it is possible that the shuffle might not be big enough and the test accuracy is not representative.
  - To fix this, when we evaluate our models, we do cross validation. This evaluates the model $n$ times and lets us avoid this problem of wondering if the test accuracy is good enough. This will give us a more accurate measure of how well a model is performing.
- Feature selection
  - When there are many features, we want to be able to find out which features are good. In this case, we used the `chi2` feature selector.
  - It is also important to not just take the feature selected values at face value and consider more or less features and test it out in practice. In our case, we found that the top 5 features were the most impactful.

## Individual Contributions

- Chua Ze Ming, [lczm](https://github.com/lczm)
- Nick Lee, [Nicklee4](https://github.com/Nicklee4)
- Madhav, [Madhav-byte-debug](https://github.com/Madhav-byte-debug)
