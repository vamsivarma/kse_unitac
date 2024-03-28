# Repository for 'Basics of Data Analysis and Visualization. Communicating Insights with Stakeholders' during KSE course supported by UNITAC and partners


# How to set up this repo - 

**Prerequisites**: You need to have Docker and Docker-compose installed on your machine 

## Settingup JupyterLab Docker

### For instantiating JupyterLab instance run the following commands

docker-compose -f docker-compose-jupyter.yml up 

**Note:** When you first run this command, it will take some time (few minutes to 15 minutes) depending on your internet connect

### To access JupyterLab instance on your browser go to following URL
localhost:8888 (passcode is **kse**)

## Settingup Solara Dashboard Docker

### To access Solara dashboard on your browser go the following URL
localhost:8765


## List of libraries configured with JupyterLab:
### Data Analysis:
Pandas, Seaborn, Plotly, Autoviz, Sweetviz

### GeoSpatial Data Analysis:
ipyleaflet, DuckDB, GeoPandas, Seaborn, Folium, shapely


## Datasets can be downloaded from:

**Note** - All the sample datasets are in the data folder

### Openbuildings dataset for Ukraine can be downloaded from DuckDB or manually from below URL
https://beta.source.coop/repositories/vida/google-microsoft-open-buildings/description/

### Datasets from Kaggle
https://www.kaggle.com/datasets?search=Ukraine

### Download Open Street Map data
https://export.hotosm.org/v3/exports/new/describe
https://www.openstreetmap.org/export#map=13/50.4585/29.8170