# CA/NV_EarthQdata
Python notebook with Maximum Likelihood estimation, linear regression, K-distance and DBScan of observed EarthQuakes in California & Nevada. This project gathers earthquake data from the USGS api, filters seismic events by magnitude & Geography, and uses machine learning to group them into clusters by event density. It calculates state level b-value (Gutenberg-richter law parameter) using a maximum likelihood estimation. Additionally, calculates b-values for each cluster by linear regression and visualizes it through an interactive folium map.  

You can edit the Api to include EQ data from any state for any measurable earthquake. However, this api has limitations in how much data can be pulled in a session. Therefore, this project will only utilize data from events between Jan 1, 1990 to June 30, 2026 in CA & NV with magnitudes >= 4.


Due to the nature of GitHub being unable to display the interactive maps, I uploaded photos of them to the "Photos_of_maps" folder. To view the interactive notebook and map without downloading this repo click the badge-->. <a target="_blank" href="https://colab.research.google.com/github/EvariG/CAEarthQdata/blob/main/CA%3ANV_seismicDBScan%26b-values_08%3A29%3A26.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a> 

Use this for other locations and analyze how crustal stress differs!


## b-values
-The lower the b-value the higher the proportion of large earthquakes to small earthquakes</p>
-A value of 1.0 indicates a proportion of 10 smaller earthquakes for 1 higher magnitude earthquake (ex. Ten 3M quakes for every One 4M quake)</p>
-The lower the b-value the more crustal stress and proportionally more larger earthquakes</p>


## Future Work and Contributions

Potential enhancements for future iterations include:

- Adding an active fault layer to the Folium maps.
- Incorporate population and housing data to explore how seismic hazard overlaps with nearby communities.
- Improving magnitude completeness estimation for each cluster.
- Adding temporal clustering to distinguish swarms, aftershock sequences, and long-term fault activity.

Contributions, suggestions, and collaborations are welcome :)


## Citation
Data source:

U.S. Geological Survey, 2017, Advanced National Seismic System (ANSS) Comprehensive Catalog, accessed via USGS API at https://earthquake.usgs.gov/fdsnws/event/1/query?format=csv&starttime=1990-01-01&endtime=2026-06-31&minlatitude=32.5&minlongitude=-124.5&maxlatitude=42.0&maxlongitude=-114.1&minmagnitude=4.0
