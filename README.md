# CA/NV_EarthQdata
Python notebook with linear regression of observed EarthQuakes in California. Dataset was gathered from the USGS EarthQuake API

You can edit the Api to include EQ data from any state for any measurable earthquake. However, this api has limitations in how much data can be pulled in a session. Therefore, I am only utilizing data from events between 1990 and June 31, 2026 in CA & NV with magnitudes greater than or equal to 4.

Use this for other locations and analyze how observed seismic events align with the Gutenberg-richter law!
<p>-The lower the b-value the smaller the ratio of small:large EQ ( and more large earthquakes compared to small ones)</p>
<p>-The lower the b-value the more potential for danger within the chosen location</p>

Due to the nature of GitHub being unable to display the interactive maps, I uploaded photos of them to the "Photos_of_maps" folder. Additionally uploaded the main ".ipynb" file to google colab. Here is the viewable link <a href="https://colab.research.google.com/drive/1ke9f2sF0-FGZ_rjee0b7MJwTmCtBJE9p?usp=sharing"> click here for Google Colab </a> 


Data source:

U.S. Geological Survey, 2017, Advanced National Seismic System (ANSS) Comprehensive Catalog, accessed via USGS API at https://earthquake.usgs.gov/fdsnws/event/1/query?format=csv&starttime=1990-01-01&endtime=2026-06-31&minlatitude=32.5&minlongitude=-124.5&maxlatitude=42.0&maxlongitude=-114.1&minmagnitude=4.0
