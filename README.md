# netCDF-degree-heating-weeks-data-analysis
Project completed as Data Analysis Research Assistant for SIO 199.

## Background 

- Raised temperatures are leading to increased frequency in warm water events, resulting in more frequent and more intense coral bleaching events.
- To understand how to quantify and measure this process, Degree Heating Weeks (DHW) are used to calculate exactly how much thermal stress a specific coral reef is under at a given time.
- A Degree Heating Week is calculated by accumulating the temperatures that are over the highest summer mean for a particular location for a specific amount of time.
- Example: if the temperature of a location is 2°C above the maximum for 4 weeks, the DHW measure is 8.
- This value can quantify how much heat has built up in that area over a long period of time.
- Worldwide temporal data is stored by the National Oceanic and Atmospheric Administration (NOAA) in a file collection, measured using Degree Heating Weeks.

## Project Goal 

The goal of this project is to utilize the NOAA file collection to conduct data analysis that will simplify complex temporal data files into a more digestible format, making the data easier to read, interpret, and wrangle.

## Data 

The data is from the lab's private database. I cannot include it in the project. Screenshots of sample data observations are available in the project poster. 

- The geographical and temporal data is all stored in a collection of NetCDF files created by the NOAA.
- NetCDF files are commonly used for storing climate data in multidimensional arrays, organized in a hierarchical manner by parameters such as coordinate locations, time, and temperature.
- Each NetCDF file contains data for a 24-hour period.
- Each file contains the DHW values for different longitude and latitude pairs across the globe for the specified day.

## Challenges 

- I had some difficulty unpacking the organizational structure of NetCDF files, due to the complexity and my unfamiliarity with the file structure.
- I had trouble accessing DHW data since so many of the values inside the array were masked.
- I initially started sampling at January 1st, which mostly contained DHW values of 0, since it is in the middle of winter, resulting in the misconception that all the values in the dataset were missing.

## Future Work 

- Generalize the data analysis onto all of the NetCDF files outside of the sample selection.
- Use the outputted CSV files to create a querying system, involving a simple interface that allows the user to query temporal data using a date and coordinate pair as query input.


