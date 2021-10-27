Coral Map
==========
This repository includes the source coude for deployment of coralmap and the machine learning  pipelines used to develop the multi-output regression model that backs coralmap's predictions.
![Unimelb logo](deployment/unimelb-logo.png "Unimelb logo")
-------------------
# Deployment
For deployment please pull deployment folder and inside your server change the directory where you saved the source code and run:
```./node_modules/.bin/pm2 start ecosystem-production.config.js --update-env --env production```
This server will start on port 3001

For further details please refer to the TerriJS documentation:
[![Docs](https://img.shields.io/badge/docs-online-blue.svg)](https://docs.terria.io/)
-------------------

This is a complete website built using the TerriaJS library. See the [TerriaJS README](https://github.com/TerriaJS/TerriaJS) for information about TerriaJS, and getting started using this repository.



For instructions on how to deploy your map, see [the documentation here](doc/deploying/deploying-to-aws.md).
# Machine Learning
