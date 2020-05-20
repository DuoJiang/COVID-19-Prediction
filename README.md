# Predicting the COVID-19 Confirmed Cases

We are a group of masters students at NYU Center for Data Science. This is a final project for the course GA-DS 1003 Introduction to Machine Learning at NYU in response to the global spread of COVID-19 virus.

The following is a detailed description of files in this repository:

* [Merge_to_Full_Dataset_git.ipynb](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/Merge_to_Full_Dataset_git.ipynb) takes in the processed dataset: 
  * [riskCalculated_confirmed_cases_moving_average_v0517_v2.csv](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/riskCalculated_confirmed_cases_moving_average_v0517_v2.csv), 
  * [cum_death_recover_update_05_08.csv](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/cum_death_recover_update_05_08.csv), 
  * [hospital.csv](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/hospital.csv),
  * [population_density_by_county.csv](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/population_density_by_county.csv) 
  
  and merges them all together to get the final dataset we used for modeling [full_data_with_hospital_MA_v0517_v2.csv](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/full_data_with_hospital_MA_v0517_v2.csv).

* [ERF error function.ipynb](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/ERF-error-function.ipynb) takes in the processed data [full_data_with_hospital_MA_v0517_v2.csv](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/full_data_with_hospital_MA_v0517_v2.csv) to fit the model and evaluate performance.

* [riskCalculation.ipynb](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/riskCalculation.ipynb) takes in the [normalized visits data](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/2020-03-01-TO-2020-04-26-visitors_home_county_normalized_v0517.csv), [population](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/reference/population_by_county.csv), and [population density](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/blob/master/data/reference/population_density_by_county.csv) by county from census, and confirmed cases data from [JHU](https://github.com/JiaruiTang/DS1003-Predicting-the-COVID-19-Cases/tree/master/data/jhu_data) to calculate the import risk of each New York county.
