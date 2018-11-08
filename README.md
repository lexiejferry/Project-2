# Project-2
A repsotiory showing a script used to automatically filter and show water quality data for the Chesapeake Bay

@Author: Lexie Ferry @Date: 2018-11-08T13:14:44-05:00 @Email: lexiejferry@gmail.com @Project: Project 2 @Last modified by: Lexie Ferry @Last modified time: 2018-11-08T13:14:44-05:00

A map showing changes in Total Dissolved Nitrate from years 2000-2017 in the chesapeake bay

Project Goal: My project goal was to see how water quality measurements for plant nutrients how changed over the years between 2000 and 2017.

About: For this project, Four maps were made, showing the level of Total Nitrates measured at water quality monitoring stations for four different years: 2000, 2006, 2012, and 2017. Time periods were chosen to be in intervals of four to show the passage of time, without adding too much data. Data was first retrieved from Chesapeakebay.net, then extracted into a point shapefile. The shapefiles were then filtered to only show Total Nitrates, and the ranges were derived automatcially to create an equal interval symbology. The maps were then put into a gif to showcase the change over the years in the Bay.

MAP



Python Code Description: The python code used was specifically designed to be able to switch between different variables for the years in the [wq2000.selectByExpression('"Parameter"=\'TN\'', QgsVectorLayer.SetSelection)] line, by simply switching out TN with a different prefered variable. The code creates a range for the variable selected and automatically assigns and Equal Interval Classification Scheme.
Python Code Used


Results: This data was not well represented by the equal interval classification scheme, and as a result the data is not easily interpretable. Using a classification scheme that equally weighs all maps on the same range would have been a better choice, but due to time constrainsts this was not possible.

Software Used: QGIS 3.2, #https://giphy.com

Data Sources:

Chesapeake Bay Program ( #http://data.chesapeakebay.net )

PyQGISDeveloper Cookbook ( #https://docs.qgis.org/testing/pdf/en/QGIS-testing-PyQGISDeveloperCookbook-en.pdf )

GIS Stack Exchange ( #https://gis.stackexchange.com/questions/100188/how-to-compute-an-interpolation-raster-from-the-python-console-in-qgis/233322 )

Author: Lexie Ferry

Date Created: 2018-11-08

Email: lexiejferry@gmail.com
