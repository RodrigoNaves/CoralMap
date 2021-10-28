Coral Map
==========
This repository includes the source coude for deployment of coralmap and the machine learning  pipelines used to develop the multi-output regression model that backs coralmap's predictions.

To access the publicly deployed version of coralmap [Go to coralmap](http://coralmap.com.au/).
![Unimelb logo](deployment/unimelb-logo.png "Unimelb logo")

# Using coralmap

1. Ensure to change your "map settings" to white and gray colours
2. Load census data by clicking "Explore map data"
3. Choose preferred dataset and "Add to the map"
4. Explore all LGA's accross Australia, see detail data by clicking on LGA area
-------------------
# Deployment
For deployment please pull deployment folder and inside your server change the directory where you saved the source code and run:
```./node_modules/.bin/pm2 start ecosystem-production.config.js --update-env --env production```
This server will start on port 3001

### For further details please refer to the TerriaJS documentation:
[![Docs](https://img.shields.io/badge/docs-online-blue.svg)](https://docs.terria.io/)
-------------------


# Machine Learning

Includes all input data used for training, and jupyter notebooks with documented preprocessing and data engineering, training of machine learning models, neural networks, and baselines.

 - ABS_data: includes cleaned and reshaped data sourced from the Australian Bureau of Statistics
- data_visualisation: Includes jupyter notebooks that will generate in-depth reports of data statistical characteristics, correlations, and distributions. The output files are in HTML format
- Deliverables: The main machine learning training and results notebook. Contains performance metrics for models trained in this project.
- Model_trianing: Details on Neural Network traning, baseline creation, and prediction ouput files
- processed_data: Outputs of the pre-processing scripts, this data were compatible datasets for time-series multioutput regression 
- Data_Preprocess_ABS_data.ipynb is the main pre-processing notebook. Most of the joins, concatenations and data standarisation is here.
- Other Auxiliary processing files: (housing data.ipynb, Data_Preprocessing.ipynb)
