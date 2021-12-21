# Kaggle-challenge-Zillow
Zillow's Home Value Prediction Kaggle Competition
![Screen Shot 2021-12-11 at 15 38 50](https://user-images.githubusercontent.com/41892953/145694998-36381f4f-8585-4ffa-843a-b9cb1d5005a2.png)

## Problem Statement
In [Kaggle Zillow challenge](https://www.kaggle.com/c/zillow-prize-1/overview/description), participants will develop an algorithm that makes predictions about the future sale prices of homes.

## Libraries
- scikit-learn
- LightGBM
- CatBoost
- Pandas
- Numpy

## Files
- [`Zillow_data_exploration_feature_extraction.ipynb`](https://github.com/wmingch1992/Kaggle-challenge-Zillow/blob/main/Zillow_data_exploration_feature_extraction.ipynb) performs basic data exploration and some feature engineering. The features are then saved to hdf5 files for later use. 
- [`Zillow_model_LightGBM.ipynb`](https://github.com/wmingch1992/Kaggle-challenge-Zillow/blob/main/Zillow_model_LightGBM.ipynb) builds [LightGBM](https://github.com/Microsoft/LightGBM) on top of the features extracted. 
- [`Zillow_model_CatBoost.ipynb`](https://github.com/wmingch1992/Kaggle-challenge-Zillow/blob/main/Zillow_model_CatBoost.ipynb) builds [CatBoost](https://github.com/catboost/catboost) models.

## Results 
| Model | Private Leaderboard Score | Private Leaderboard Ranking | 
| :---: | :---:| :---: | 
| LightGBM | 0.07511 | 215 / 3770 | 
| CatBoost | 0.07521 | 420 / 3770 | 
| **Average (LightGBM + CatBoost)** | **0.07500** | **82 / 3770** |

- LightGBM and CatBoost have similar performance 
- After doing the simple avearge for LightGBM and CatBoost (same weight), the performance is improved substantially. 

