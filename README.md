# Duke_510_Project
Attendance Prediction of Duke Sporting Events. 

## Project Overview
Predictions for men's football and women's basketball home game attendance from 2016-2023. Training data is from 2016 - 2021. Data from 2022 onwards used for test set. 

## Code Overview
Code involved sourcing data from a weather API, as well as web scraping for sports dates and scores 

## Process
1) Sourced Data from Various Websites
      - attendance_fb.ipynb (attendance_fb.py)
      - attendance_wb.ipynb (attendance_wb.py)
      - calendar_dates.ipynb (calendar_dates.py)
      - weather.ipynb (get_weather_data.py)
2) Merging Data Into One File and Performing Initial Cleaning
      - Merge Dataset.py
3) Performed EDA on Data
      - make_charts.ipynb 
4) Second Cleaning of Data and Feature Engineering Before Modeling
      - data_functions.py
5) Modeling & Model Evaluation 
      - model_functions.py
   
## Notebooks
Notebooks were used for exploration before solidifying code into .py scripts.

### attendance_fb.ipynb
Pulled football attendance data, and relevant game data from wikipedia using web scraping.

### attendance_wb.ipynb
Pulled women's basketball attendance data, and relevant game data from wikipedia using web scraping.

### calendar_dates.ipynb
Pulled academic calendar data and classified dates as "holiday", "exam", or "class" for use in model 

### weather.ipynb
Used API to obtain weather data for Duke Men's Football and Women's Basketball gamedays between 2016 - 2023 

### make_charts.ipynb
Performing exploratory data analysis and generating plots used in presentation 


## Scripts
Scripts pull and manipulate data using functions. Some initial data updates were done external to scripts, since the data set was so small and manual updates took seconds to complete (vs extended time in code).

### attendance_fb.py
Pulled football attendance data, and relevant game data from wikipedia using web scraping.

### attendance_wb.py
Pulled women's basketball attendance data, and relevant game data from wikipedia using web scraping.

### calendar_dates.py
Pulled academic calendar data and classified dates as "holiday", "exam", or "class" for use in model 

### get_weather_data.py
Used API to obtain weather data for Duke Men's Football and Women's Basketball gamedays between 2016 - 2023 

### Merging.py
Merging sourced datasets into aggregate dataset and performing intial cleaning steps 

### data_functions.py
Pulling in aggregated dataset and performing further cleaning steps and feature engineering 

### model_functions.py
Using final dataset from data_functions.py and training a random forest regression on training data (2016 - 2021) and evaluating model metrics on test dataset (2022 onwards) 
