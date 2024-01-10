
# About

AG2417 PROJECT: urban Green prediction based on senitinel2 sensor data

## 1 Dataset download

The HARMONIA urban green dataset can be downloaded from Zenodo.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10210237.svg)](https://doi.org/10.5281/zenodo.10210237)

## 2 Network training

To train the network, run the ``train_network.py`` file with the ``optical.yaml`` config:

````
python 'D:/study documents/GIS_project/code/HARMONIA_urban_green-master/HARMONIA_urban_green-master/train_mapping.py' -c 'D:/study documents/GIS_project/code/HARMONIA_urban_green-master/HARMONIA_urban_green-master/configs/optical.yaml' -o 'D:/study documents/GIS_project/code/HARMONIA_urban_green-master/HARMONIA_urban_green-master/output' -d 'D:/study documents/GIS_project/code/HARMONIA_urban_green-master/HARMONIA_urban_green-master/dataset' -p 'wandb project for logging'
````

## 3 Inference


Run the files ``inference.py`` for one of the four pilot cities.

````
python inference.py -c optical -s 'pilot city' -y 'reference year' -o 'path to output directory' -d 'path to the dataset'
````

# Funding
 
This work is funded by the  EU Horizon 2020 project HARMONIA (Grant agreement ID: 101003517). Please find more information on the [HARMONIA website](https://harmonia-project.eu/). 
