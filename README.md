# Spaceship

- [x] Write problem definition
- [x] Data preparation
- [x] Data cleaning
- [x] Exploratory data analysis
- [x] Exploratory data visualization
- [x] Build a model
- [ ] Verify the model
  - [ ] Fine-tune the model
- [x] Something new from the course
  - Sampling techniques
  - Cross validation techniques
  - Feature selection
  - SVC

# SC1015 Data Science Project

## Problem Definition

Given this ["Key Indicators of Heart Disease" dataset](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease), which has many various indicators, we want to build a model that can use these indicators, that any regular adult can obtain through a health screening, to evaluate the risk that any given individual has for heart disease.

##

## Conclusion

- We are able to evaluate risk of a given individual with reasonable accuracy.
- There are many factors that are highly correlated with heart disease.
  - Physical Health Days and Having Angina (Type of chest pain) are major indicators.

## Learning Outcomes

- Handling a massively imbalanced dataset (1:24)
  - Undersampling can remove key features. Even when randomly sampling, we cannot just look at how many rows of data we have for the minority class. How many columns / factors of data we have also matter. In the case of this dataset, we have a lot of columns and we lost features through undersampling.
- KFold Cross Validation
  - TODO
- Feature selection
  - TODO

## Individual Contributions

- Chua Ze Ming, [lczm](https://github.com/lczm)
- Nick Lee, [Nicklee4](https://github.com/Nicklee4)
- Madhav, [Madhav-byte-debug](https://github.com/Madhav-byte-debug)
