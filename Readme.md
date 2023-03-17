# GoDaddy - Microbusiness Density Forecasting competition 

Competition name: GoDaddy - Microbusiness Density Forecasting

[Kaggle competition](https://www.kaggle.com/competitions/godaddy-microbusiness-density-forecasting/overview) 

### Description in short:
  * "The goal of this competition is to predict monthly microbusiness density in a given area."
  * 3135 counties of U.S. are used for predicting microbusiness density
  * "Microbusinesses are generally defined as businesses with an online presence and ten or fewer employees"
  * Godaddy collected information on these businesses.
  * Correct competition test data consists of months: march,april and may of 2023, while ignoring january and ferbruary.
### Data in short:
  * Data (mainly) consist of microbusiness density from 2019.08.01 to 2022.10.01. per month, for each county.
  * The goal is to predict microbusiness density for march,april and may of 2023, while ignoring january,ferbruary and June.
  * Data are available at [kaggle](https://www.kaggle.com/competitions/godaddy-microbusiness-density-forecasting/data)
  
  Note: June is added by mistake in test.csv data. January was used as test during competition (public leaderboard). Only march,april and may of 2023 will be used for determining final score. Competition will probably end after May data are available for scoring.

  Note: Data from train.csv and additional data from revealed_test.csv should be concatenated and used for training.
## What is done:
  1. split-data.ipynb - Data is cleaned from outliers and split into convinient parts to be used for training,validation and creating submission.
  2. prepare-data.ipynb - Feature egineering.
  3. model.ipynb - Pytorch model is trained and evaluated.
  4. create-submission.ipynb - Submission is created and prediction adjusted for low population counties.
