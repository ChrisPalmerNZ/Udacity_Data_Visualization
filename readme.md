# Ford GoBike / Lyft Bay Wheels Data Exploration

## Dataset

The data consists of some 5.8 million records, consisting of time, geographical and user-type information of individual trips, from June 2017 until March 2020. There is no subscriber identification and little customer-specific information, except for gender and birth year information collected from June 2017 to April 2019.

Data was obtained from the [archives](https://s3.amazonaws.com/baywheels-data/index.html) linked to from the [System Data](https://www.fordgobike.com/system-data) page of the Lyft Bikes web site. Here the data consists of a number of CSV files in zip archives. 

Data was downloaded, extracted, combined and augmented with extra features to aid analysis. and saved into a SQLite database - which is around 3 GB in size. The database file is named fordgobike.db.


## Summary of Findings

During data exploration and the subsequent data explanation notebooks the most significant finding was a large variability in patronage of the Ford GoBike / Lyft Bay Wheels service. Some of this could be linked to availability of e-bikes, but it seems most certainly to be related to pricing changes, culminating in what looks like a drastic downturn in the usage for the final month of the data, March 2020.

The data analysis makes it clear that the most important users are Subscribers, and that at the end of the available data that they have deserted the service in large numbers.

## Key Insights for Presentation

The data analysis is presented in the form of a slide show, which initially examines  information about the fluctuations and downturn of patronage using trip counts analysis, and in its conclusion by using geographical analysis.

Along the way the presentation includes data analysis of the main data points, so that a clear picture emerges of customer demographics.

## Notebooks

There are four notebooks involved, in order of their development:

1. Data\_Visualization\_Project_DataSetup.ipynb - used to extract the data from the CSV files and save it into a SQLite database
2. Data\_Visualization\_Project\_DataExploration.ipynb - used to explore and describe the data, and to add features that aid analysis. The enhanced data is then saved into a new table in the database, ready for explanatory data analysis.
3. Data\_Visualization\_Project\_DataExplanation.ipynb - used to conduct the explanatory data analysis an construct visuals, including various permutations of some of the charts.
4. Data\_Visualization\_Project\_DataExplanation_Slides.ipynb - a version of the exlpanatory notebook reorganized and dedicated to presenting the insights as a slide show.   

