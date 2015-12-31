# Visualized statistics on income per dutch postcode

[See result](http://jvdm.info/postcode/inkomen.html)

## Background
Interested in statistics and really wanting to learn d3.js visualizations
For more background see:  http://janvandermeiden.blogspot.nl/

## History
Downloaded postcode maps from:
curl http://geoplaza.vu.nl/data//dataset/8b484bab-78e7-4687-9a2b-a8321fe0b58d/resource/3874f60f-e9a1-49b0-b0a8-a3e7d282c969/download/esri-openpostcodevlakkenpc4.zip
The credit for this data goes to: ESRI Nederland http://www.esri.nl/

Converted Dutch postcode data to topojson:
ogr2ogr   -f GeoJSON   postcode4.json   ESRI-PC4-2015R1.shp
topojson -o pc4NL.json --id-property PC4 --properties geometry -- postcode4.json
The credit for this conversion goes to GDAL http://www.gdal.org and Mike Bostock, especiallyi this article: http://bost.ocks.org/mike/map/

Downloaded CBS data on income via:
http://www.cbs.nl/nl-NL/menu/themas/dossiers/nederland-regionaal/cijfers/incidenteel/maatwerk/default.htm
The credit for this data goes to CBS http://www.cbs.nl



## Current status
Work in progress
