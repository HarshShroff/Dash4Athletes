# Introduction

Fitness plays a major role, especially for the professional athletes who keep track of it. The suggested methodology introduces the detailed analysis of bicyclists’ performance.
Strava, a mobile application can track user’s activity like walking, swimming, and cycling and provides basics information like speed, distance, and elevation. This project describes the similar activity dashboard with different approach for analysing the bicyclists’ activity.
For the dataset, the data from a long term Strava user consisting of _.GPX_ and _.CSV_ files is used. Various pre-processing and calculation methods are applied like imputation, row and column filtering, calculating exact speed and distance from the _.GPX_ file, splitting the pair of GPS coordinates in two to calculate to-and-fro routes, mapping of selected route and separating the year and month from the timestamp to calculate date, time and day of the activity to provide monthly, yearly and weekly analysis of users’ activity.

# Data Analysis

When it comes to data analysis, data cleansing is necessary. Unwanted data, files with garbage and incorrect data, must be removed, leading to a hazel-free analysis.

The following steps were undertaken for data filtering:
* Reading the _activities.csv_ file as a Pandas dataframe,
* extracting the total rows and columns of the dataframe,
* getting the list of all columns from the dataframe,
* removing unwanted and null rows and columns,
* calculating different parameters from the GPX file,
* and lastly visualizing all of these gathered information in an appropriate manner.

GPX, or GPS Exchange Format, is an XML schema designed as a common GPS data format for software applications. It is used to describe way-points, tracks, and routes.
Processing GPX file does not seem too hard but there are a few trap-holes which can be overcome by applying different types of mathematical formulae on it.

# Data Visualization

Using interactive graphs and maps, the final processed data was used to display the analysis in a suitable storytelling fashion. **Plotly Express**, a Python module, is used to do so, while **Dash**, another Python module, is used to visualize the graphs on a web browser.

# Dashboard

## Overview

![](https://github.com/HarshShroff/Dash4Athletes/blob/main/imgs/Screenshot%20(44).png)
![](https://github.com/HarshShroff/Dash4Athletes/blob/main/imgs/Screenshot%20(45).png)
![](https://github.com/HarshShroff/Dash4Athletes/blob/main/imgs/Screenshot%20(46).png)
![](https://github.com/HarshShroff/Dash4Athletes/blob/main/imgs/year.png)

## Video Explanation
<a href="https://youtu.be/gvnl0ZfR4DM?t=653" target="_blank">
 <img src="http://img.youtube.com/vi/gvnl0ZfR4DM/hqdefault.jpg" alt="Watch the video"  border="10" />
</a>
