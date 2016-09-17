# RNI-Activity-Expenses


This repository contains a dataset detailing expenses for activities that were conducted as part of [Ushahidi](https://www.ushahidi.com)'s [Resilience Network Initiative](http://cityresilience.net/what-is-rni.html) ("RNI") in Indonesia.

##Data
The [data folder](https://github.com/Shadrock/RNI-Activity-Expenses/tree/master/data) contains:
* A polygon to denote the [boundaries of the neighborhood of Purwodinatan] (Data/Purwodinatan%20Neighborhood%20Project%20Area.geojson), which was the focus of our work in Semarang, Indonesia. You can learn more about that project [in this video](https://vimeo.com/129603769) and [this blog post](http://www.100resilientcities.org/blog/entry/kathmandu-semarang-citizen-engagement-and-open-data-mapping-in-two-cities#/-_/).
* A complete [list of **all** expenses](data/RNI IND Project Expenditures 2014-2015.json) associated with RNI's work in Indonesia in the JSON format. [JSON](http://www.json.org/), which is a great open standard data format. 
* A complete [list of **all** expenses](data/RNI IND Project Expenditures 2014-2015.csv) associated with RNI's work in Indonesia in a table... for those who like that sort of thing. 

Note that...

These data were created and used primarily as a method of real-time reporting to donors and other stakeholders and to document events that were of importance to complete various aspects of the overall project. Data were created using the Ushahidi platform ([Github here](https://github.com/ushahidi/platform) | [project deployment here](http://rni.ushahidi.com)) and replicated in the OpenExplorer platform ([project deployment here](https://openexplorer.com/expedition/rnix)) to provide multiple ways of interacting with the data. 

Because this type of reporting was _not_ a requirement for this project, there is no overarching definition of what constitutes an ‘activity.’ Some records may indicate a discreet event such as a contract signing, while others may denote the culmination of a series of discreet events that led to a project milestone or deliverable, such as the completion of a neighborhood map. We see this dataset as an example of the granularity that is possible for reporting and how we can be more open and transparent about how and where we work. This is a work in progress for us and I welcome feedback on how data creation of this type can be improved for various uses.  

## Data Creation Process for this Repository
The following steps were taken to convert data from an Ushahidi deployment (version 2) for this repository.

1. Downloaded data from the [Ushahidi deployment](http://rni.ushahidi.com).
2. Previewed data and corrected diacritical marks and other typographic symbols that did not display correctly in a spreadsheet editor. Also added the geographic precision code, which is part of a custom form in the Ushahidi deployment that did not automatically appear in the report download. 
3. Because older Ushahidi deployments commonly offer .csv as a download default, I used [this tool] (http://www.convertcsv.com/csv-to-geojson.htm) to convert .csv to GeoJSON.
4. Previewed and cleaned up resultant code with [Mapbox's](https://www.mapbox.com/) [geojson.io](http://geojson.io), which also allowed me to...
5. save code directly to Github. 

Additionally, Mapbox has another [handy tool](http://mapbox.github.io/togeojson/) for converting .gpx files to GeoJSON.


