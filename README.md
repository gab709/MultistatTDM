# MultistatTDM

Authors
Daniele Ortu, Gabriele Merlin
University of Cagliari 

MultistatTDM is a modified version of Grafana’s native multistat panel. It is a part of TDM project, (link: http://www.tdm-project.it/), initiative born thanks to the collaboration between CRS4 and University of Cagliari.
In this case, the goal was to show the measurements of many electric appliances, provided by Iotawatt sensor. Users could see through this panel the actual consumption or a mean.

Original version of SingleStat Panel
Read more about it here:
https://grafana.com/grafana/plugins/michaeldmoore-multistat-panel

###################
Limits of native panel
###################

The original panel provides the possibility to insert only 1 query. The returned data are a list of measurements (see the documentation for more specific details), which are displayed in the form of bar graphs with optional upper and lower hard limits. There isn’t the possibility to manage a data to display in the graphs the values of its column.
Another limit is the absence of the possibility to insert other dynamic indicators in the columns, such as mean, min, and max.

###################
What’s new?
###################

This modified version allows you to manage only one result, displaying the measurements of each column in the graph. Once the first query is inserted, there is the possibility to define the label of each bar. The N bar is the N column of the unique result of the query, without considering the first column of timestamp.
There is also the possibility to insert a second query to provide a list of dynamic values showed in the graph. 

###################
Setup on Grafana(Windows)
###################

To use this plugin inside grafana it is necessary to download it, unzip it and insert it into the grafana installation folder: grafana-5.4.2 -> data -> plugins 
To configure it on grafana you need the support to a database as influxdb or similar.



