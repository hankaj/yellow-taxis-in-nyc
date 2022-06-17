# S07. Yellow Taxis in NYC

## Authors:

* Kamil Barszczak
* Hanna Jarlaczyńska
* Konrad Pawlik

## Scripts' main goal and theirs executing order
* 0 - [Download Data](https://gitlab.kis.agh.edu.pl/data-engineering-2022/s07-yellow-taxis-in-nyc/-/blob/main/notebooks/download_data.ipynb) - Downloading required 2018-taxi-trip-data (We advise to download dataset directly from https://data.cityofnewyork.us/api/views/t29m-gskq/rows.csv?accessType=DOWNLOAD link and putting .csv file into a resources directory, as it is faster solution)
* 1 - [Data Processing](https://gitlab.kis.agh.edu.pl/data-engineering-2022/s07-yellow-taxis-in-nyc/-/blob/main/notebooks/data_processing.ipynb) - Renaming columns, getting rid of redundant ones and transforming day of week/time values into ML-ready.
* 2 - [Data Visualization](https://gitlab.kis.agh.edu.pl/data-engineering-2022/s07-yellow-taxis-in-nyc/-/blob/main/notebooks/data_visualization.ipynb) - Visualizing number of pickups in each taxi zone.
* 3 - [Road Lenghts](https://gitlab.kis.agh.edu.pl/data-engineering-2022/s07-yellow-taxis-in-nyc/-/blob/main/notebooks/road_lenghts.ipynb) - Calculating sum of road lengths in each taxi zone.
* 4 - [Merge Datasets](https://gitlab.kis.agh.edu.pl/data-engineering-2022/s07-yellow-taxis-in-nyc/-/blob/main/notebooks/merge_datasets.ipynb) - Merging taxi data with road lenghts and calculating probability of pickup/dropoff for each zone, day of week and hour.
* 5 - [ML Models](https://gitlab.kis.agh.edu.pl/data-engineering-2022/s07-yellow-taxis-in-nyc/-/blob/main/notebooks/ml_models.ipynb) - training SGDRegressor models to predict a number of passengers and XGBRegressor to predict a probability of pickup/dropoff.

## Catalogs description:

* notebooks - the catalog for jupyter lab scripts that are used to prepare the final dataset.
* processed_data - the catalog is used to store the final processed dataset.
* resource - the catalog contains data used to get the final dataset. For example taxi zones in NY city.


