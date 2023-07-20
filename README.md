<<<<<<< HEAD
# Project1Group8

This repo contains the first group assignment for group 8: Priya, Raviska, Sagar and Rhiannyn

# The folders and files in reading order are as follows:
1. Cleaning_Merging_Raw_data contains 
- the csv files of the original datasources (1.world-data-2023_original_raw, co2_emission_years, death_air_pollution) - See REFERENCES below for reference details
- two Jupyter files : 1st_Jupyter_file_world_data_2023_cleanup, and Merged_Data_Sources, for the basic cleanup to arrive at - organised_world_data.csv 

2.  World_Air_Quality_Data.ipynb - the jupyter file to pull the air quality data API request for the dataset

3.  final_merged_world_data.csv - the cleaned, merged, shared file that makes up the basis of the first stage of the analysis.

4. Airquality_deaths_bar_box_charts.ipynb: python file for the charts for slides 4 & 5

5. Air_Pollution_Plots.ipynb: python file for the chart on slide 10, and the geospatial visualisation for slide 11

6. bokeh5kj76ri8.html : the html link for the geospatial visualisation for slide 11 

7. Airpollution_data_py.ipynb: creating the additional csv for processing co2 and deaths over years (section 2 of the analysis)

8. GDP_vs_CO2_Analysis.ipynb: python file for charts on slides 12 - 14 

9 - 12. Our resources and output files
Priya_Output & Priya_Resources - including output files for slides 3, 10 & 11 
Rhiannyn_Output & Rhiannyn_Resources - including pngs for slides 4 & 5
Raviska_Outputs & Raviska_Resources - includes three python files: Air_Pollution_Pie_Plots.ipynb, co2_emission_years_line_chart.ipynb, Merging Data Frames.ipynb, for the creation of the charts on slides 6 -9.  
Sagar_Output & Sagar_Resources - including output pngs for slides 12-14


# Steps that were undertaken 
Step 1 – Select Project Topic: Changes in worldwide air quality
Step 2 - Identifying Data sources
2.	air pollution deaths
3.	Annual-co2-emissions-per-country
4.	Air pollution data by year: from Open Weather API 
5.	Co2 Emission by year 
6.	GDP by year 

Step 3 - merging, cleaning and processing data using excel, jupyter notebook and python
-	Reading csv into pandas
-	Reordering columns 
-	Removing irrelevant columns
-	Renamed columns
-	Checked row counts and type for each columns
-	Changed data types where required to be suitable for data comparison
-	Dropped rows with incomplete data
-	Set index as country
-	Wrote to csv 

Step 4: Research Questions and Visualisations
- creating and adapting the charts based on research questions 

Step 5: PPT development and presentation
Project Introduction (Rhiannyn)
Air pollutants and the AQI: Top 5 countries by air pollutants other than Co2 – the “top 5 worst pollutants” list (Rhiannyn) & Deaths by Air pollution
Bar graph of top 5 countries, graph of the air pollutants and death rates: is there a statistically relevant link?

Understanding the link between C02 emissions and the causing impact on death? (Raviska)

Which countries have the highest and lowest C02  emissions from 2000 to 2021? (Raviska)
How are countries world wide rated according to AQI (Air Quality Index)?

Can we measure countries’ economic prosperity according to environmental impact? 
Variables being measured: GDP against CO2 emissions: is there a correlation? (Sagar)
Scatterplot & Line graph

Average CO₂ Emission in Billion tonnes per Year and how is has been varying over years (Priya)
Line/Histograph
Air Quality and CO2 Emission in the Year 2021 across 166 Countries (Priya)
Geomap


# REFERENCES and DATASOURCES
1.	organised_world_data.csv data from “World Data 2023 dataset”, https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023, Author: NIDULA ELGIRIYEWITHANA, accessed 11/7/2023
2.	air pollution deaths: https://www.kaggle.com/datasets/akshat0giri/death-due-to-air-pollution-19902017, , author: AKSHAT_GIRI, accessed 15/7/2023
3.	Annual-co2-emissions-per-country: https://ourworldindata.org/co2-dataset-sources
4.	Air pollution data by year: from Open Weather API (Lat/Lon: http://api.openweathermap.org/data/2.5/weather? & Air Pollutants: http://api.openweathermap.org/data/2.5/air_pollution?) for air pollutants & Lat/Lon. The requests were made based on the merged data list of countries and capital cities. 
5.	Co2 Emission by year csvdata from: CO2 Emission by countries Year wise (1750-2022), https://www.kaggle.com/datasets/moazzimalibhatti/co2-emission-by-countries-year-wise-17502022, authors: MOAZZIM ALI BHATTI, EMMANUEL MADANGA, accessed 13/7/23
6.	GDP by year csv file data from: PIB-GDP Global by countries since 1960 to 2021,  https://www.kaggle.com/datasets/fredericksalazar/pib-gdp-global-by-countries-since-1960-to-2021,  author: FREDERICK ADOLFO SALAZAR SANCHEZ, accessed 15/7/2023


=======
# Project1Group8


Step 1 – Select Project Topic: Changes in worldwide air quality

Step 2 - Identifying Data sources

1.	organised_world_data.csv data from “World Data 2023 dataset”, https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023, Author: NIDULA ELGIRIYEWITHANA, accessed 11/7/2023
2.	air pollution deaths: https://www.kaggle.com/datasets/akshat0giri/death-due-to-air-pollution-19902017, , author: AKSHAT_GIRI, accessed 15/7/2023
3.	Annual-co2-emissions-per-country: https://ourworldindata.org/co2-dataset-sources
4.	Air pollution data by year: from Open Weather API (Lat/Lon: http://api.openweathermap.org/data/2.5/weather? & Air Pollutants: http://api.openweathermap.org/data/2.5/air_pollution?) for air pollutants & Lat/Lon. The requests were made based on the merged data list of countries and capital cities. 
5.	Co2 Emission by year csvdata from: CO2 Emission by countries Year wise (1750-2022), https://www.kaggle.com/datasets/moazzimalibhatti/co2-emission-by-countries-year-wise-17502022, authors: MOAZZIM ALI BHATTI, EMMANUEL MADANGA, accessed 13/7/23
6.	GDP by year csv file data from: PIB-GDP Global by countries since 1960 to 2021,  https://www.kaggle.com/datasets/fredericksalazar/pib-gdp-global-by-countries-since-1960-to-2021,  author: FREDERICK ADOLFO SALAZAR SANCHEZ, accessed 15/7/2023


Step 2 - merging, cleaning and processing data using excel, jupyter notebook and python
-	Reading csv into pandas
-	Reordering columns 
-	Removing irrelevant columns
-	Renamed columns
-	Checked row counts and type for each columns
-	Changed data types where required to be suitable for data comparison
-	Dropped rows with incomplete data
-	Set index as country
-	Wrote to csv 

Files used for cleaning processes:
-	world_data_2023_cleanup.ipynb
-	include list RG to do
- 	Merge_Data_sources(use full name)


Step 3: Research Questions and Visualisations
File name/s, image name/s

Project Introduction (Rhiannyn)
Air pollutants and the AQI: Top 5 countries by air pollutants other than Co2 – the “top 5 worst pollutants” list (Rhiannyn) & Deaths by Air pollution
Bar graph of top 5 countries, graph of the air pollutants

Understanding the link between C02 emissions and the causing impact on death? (Raviska)

Which countries have the highest and lowest C02  emissions from 2000 to 2021? (Raviska)
How are countries world wide rated according to AQI (Air Quality Index)?

Can we measure countries’ economic prosperity according to environmental impact? 
Variables being measured: GDP against CO2 emissions: is there a correlation? (Sagar)
Scatterplot & Line graph

Average CO₂ Emission in Billion tonnes per Year and how is has been varying over years (Priya)
Line/Histograph
Air Quality and CO2 Emission in the Year 2021 across 166 Countries (Priya)
Geomap


Presentation - Speaker order:
Rhiannyn: Introduction & air pollutants
Raviska, 
Priya, 
Sagar: Co2 and GDP, and concluding remarks


List of files and order to be read:

List of images from presentation:



>>>>>>> parent of 1c291cb (Update README.md)
