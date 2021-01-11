README:

program: mta_women_tech_gala_final_CCHAN.ipynb
date modified:01/08/2021
team: Group 5 (Joshua Banks, Humza Khan, Chuck Cao, Chris Chan)
this specific program created by: Chris Chan

PURPOSE:

The purpose of the project is to analyze the NYC MTA data (and other sources) to
determine the most effective/efficient strategy to canvas NYC subways to raise 
awareness and funding for Women's Tech Women's Yes organization.

Our analysis focused on 2 primary strategies. 
1. Focus on tech areas based on data and domain knowledge. This captures highest interest individuals.
2. Focus on high income areas to raise funding. This captures individuals who can provide funding


PROGRAM OUTLINE:

Each team member contributed greatly to the overall code and end product. 
Each member maintained their own programs and worked on separate pieces, therefore
the "data prep" portion has the most overlap between programs given we are all starting from the same 
analytic dataframe. 

The outline below walks through this program and highlights the specific sections that I worked on.
The sections I worked on have "**" before the section number:

1. Prep MTA Turnstile data
	. read-in, clean MTA turnstile data for 4 months of July 2019

2. Prep Stations Data
	. read-in station level data with lat/lng info used for mapping to income

**3. (cchan): Adding Income Data to Stations by Lat/Lng
	. import "uszipcode" python package to use search function based on our list
		of lat/lng data. This package allowed us to hit a compiled database
		containing geo level data (lat/lng) along with demographic and economic data
	. this is how we obtained median hh income   

**4. (cchan): Merge Stations (with income) to Turnstile DF
	. Used a crosswalk between the MTA turnstile data and MTA stations data to link
		the files together. 

5. Clean merged station, turnstile and income data and product final analytic DF

6. Analyze data using visuals

6a. Graphs for overall traffic in NYC (Humza Khan)

6b. Graphs for Tech+Income in NYC (Joshua Banks)

**6c. (cchan): Graphs for high income
	. original graphs used for presentation on 01/08/2021

**7. (cchan): Attempts to improve maps
	. new graphs used in most recent ppt presentation. The improvement was to 
		 more accurately and cleanly represent the subway station level income,traffic
		 data points onto a map of manhattan
	. these new graphs deploy geopandas to create the underlying nyc maps
	. this was not incorporated orginally due to time and simply lack of knowledge
	. these are now updated based on feedback from METIS instructors

**8. (cchan): Testing code
	. this is just a copy of test code throughout the process


** END OF readme **
