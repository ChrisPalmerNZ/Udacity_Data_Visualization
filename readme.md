# Ford GoBike / Lyft Bay Wheels Data Exploration

## Dataset

The data consists of some 5.8 million records, consisting of time, geographical and user-type information of individual trips, from June 2017 until March 2020. There is no subscriber identification and little customer-specific information, except for gender and birth year information collected from June 2017 to April 2019.

Data was obtained from the [archives](https://s3.amazonaws.com/baywheels-data/index.html) linked to from the [System Data](https://www.fordgobike.com/system-data) page of the Lyft Bikes web site. Here the data consists of a number of CSV files in zip archives. 

Data was downloaded, extracted, combined and augmented with extra features to aid analysis. and saved into a SQLite database - which is around 3 GB in size. The database file is named fordgobike.db.


## Summary of Findings

During data exploration and the subsequent data explanation notebooks the most significant finding was a large variability in patronage of the Ford GoBike / Lyft Bay Wheels service. Some of this could be linked to availability of e-bikes, but it seems most certainly to be related to pricing changes, culminating in what looks like a **_drastic downturn_** in the usage for the final month of the data, March 2020.

The data analysis makes it clear that the most important users are Subscribers, and that at the end of the available data that they have deserted the service in large numbers.

## Key Insights for Presentation

The data analysis is presented in the form of a slide show, which initially examines  information about the fluctuations and downturn of patronage using trip counts analysis, and in its conclusion by using geographical analysis.

Along the way the presentation includes data analysis of the main data points, so that a clear picture emerges of customer demographics, especially the importance of subscribers.

The concluding example in the analysis demonstrates the downturn in subscriber numbers by comparing images and numbers of trip information for three Wednesdays in March - one each in 2018, 2019 and 2020. It shows that the 2020 subscriber numbers at 1,847 are half those of the 2018 numbers which were at 3,622, and a quarter of of the preceding 2019 year which were at 8,152. 

## Notebooks and Slide show

There are four notebooks involved, in order of their development:

1. [Data\\_Visualization\\_Project_DataSetup.ipynb](https://github.com/ChrisPalmerNZ/Udacity_Data_Visualization/blob/master/Data_Visualization_Project_DataSetup.ipynb) - used to extract the data from the CSV files and save it into a SQLite database
2. [Data\\_Visualization\\_Project\\_DataExploration.ipynb](https://github.com/ChrisPalmerNZ/Udacity_Data_Visualization/blob/master/Data_Visualization_Project_DataExploration.ipynb) - used to explore and describe the data, and to add features that aid analysis. The enhanced data is then saved into a new table in the database, ready for explanatory data analysis.
3. [Data\\_Visualization\\_Project\\_DataExplanation.ipynb](https://github.com/ChrisPalmerNZ/Udacity_Data_Visualization/blob/master/Data_Visualization_Project_DataExplanation.ipynb) - used to conduct the explanatory data analysis an construct visuals, including various permutations of some of the charts.
4. [Data\\_Visualization\\_Project\\_DataExplanation\\_Slides.ipynb](https://github.com/ChrisPalmerNZ/Udacity_Data_Visualization/blob/master/Data_Visualization_Project_DataExplanation_Slides.ipynb) - a version of the exlpanatory notebook reorganized and dedicated to presenting the insights as a slide show.   
5. [The slide show](https://github.com/ChrisPalmerNZ/Udacity_Data_Visualization/blob/master/Data_Visualization_Project_DataExplanation_Slides.slides.html)

## Geographical Analysis

The Uber [kepler.gl](kepler.gl) geospatial analysis tool was used for the geographical analysis. Animations were recorded using [ScreenToGif](screentogif.com).  


