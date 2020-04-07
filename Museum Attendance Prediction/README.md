# Museum Attendance Prediction

## General Introduction
This is part of my work for my practicum project, which is to build predictive model for the museum's daily attendance.
Due to the condifential issue, the codes won't include any data. 

## Data Process
I have mainly two parts of data, the first part is the information about museum's special exhibits and the second part is the external data I scraped from public website, like the crime and weather data.

I have first transformed the exhibit-level data into the daily-level and then aggregated the weather data into the dataset.
For aggregation methods, I have used min, max, mean, median values.
Apart from this, I have added some features that can reflect the historical trends, like moving average.

## Modeling
I have constructed a Random Forest model model using random search for parameters tuning. 
Random Forest workds really well in this case because there are some key factors that are influcing the attendance, such as the museum is closed on Monday so attendance for every Monday is 0. And RF can classify all the Mondays into the same section and make proper prediction.
The predictive model results in a 0.74 R-squared in the test set.

## Recommendations and Insights
After building the model, I extracted some important features and conduct analysis on those features. It turns out exhibits with a story or pre-modern exhibits are more attractive to visitors compared to other features.
It would be better if the museum can consider hosting those exhibits to draw more visitors.

## Authors

**Han(Shuhan) Lu** - *Initial work* - [LinkedIn page](https://www.linkedin.com/in/shuhan-lu/) - [Medium page](https://medium.com/@lushuhan95)
