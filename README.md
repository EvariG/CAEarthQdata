# CA/NV_EarthQdata
Python notebook with Maximum Likelihood estimation, linear regression, K-distance and DBScan of observed EarthQuakes in California & Nevada. This project gathers earthquake data from the USGS api, filters seismic events by magnitude & Geography, and uses machine learning to group them into clusters by event density. It calculates state level b-value (Gutenberg-richter law parameter) using a maximum likelihood estimation. Additionally, calculates b-values for each cluster by linear regression and visualizes it through an interactive folium map.  

You can edit the Api to include EQ data from any state for any measurable earthquake. However, this api has limitations in how much data can be pulled in a session. Therefore, this project will only utilize data from events between Jan 1, 1990 to June 30, 2026 in CA & NV with magnitudes >= 4.

Use this for other locations and analyze how crustal stress differs!

-The lower the b-value the higher the proportion of large earthquakes to small earthquakes</p>
-A value of 1.0 indicates a ratio or 10 smaller earthquakes for 1 higher magnitude earthquake (ex. 10 3M quakes for every 1 4M quake)</p>
-The lower the b-value the more crustal stress and proportionally more larger earthquakes</p>

Due to the nature of GitHub being unable to display the interactive maps, I uploaded photos of them to the "Photos_of_maps" folder. Additionally uploaded the main ".ipynb" file to google colab. Here is the viewable link <a href="https://colab.research.google.com/drive/1ke9f2sF0-FGZ_rjee0b7MJwTmCtBJE9p?usp=sharing"> CA:NV_seismicDBScan&b_values </a> 


## Future Work and Contributions

Potential enhancements for future iterations include:

- Adding an active fault layer to the Folium maps.
- Incorporate population and housing data to explore how seismic hazard overlaps with nearby communities.
- Improving magnitude completeness estimation for each cluster.
- Adding temporal clustering to distinguish swarms, aftershock sequences, and long-term fault activity.

Contributions, suggestions, and collaborations are welcome. :)



Data source:

U.S. Geological Survey, 2017, Advanced National Seismic System (ANSS) Comprehensive Catalog, accessed via USGS API at https://earthquake.usgs.gov/fdsnws/event/1/query?format=csv&starttime=1990-01-01&endtime=2026-06-31&minlatitude=32.5&minlongitude=-124.5&maxlatitude=42.0&maxlongitude=-114.1&minmagnitude=4.0
