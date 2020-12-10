# Operationalizing Machine Learning

This project is part of the Udacity Azure ML Nanodegree. In this project, we will be working on with the Bank Marketing dataset, which contains data about the personal and financial details of customers in a Portugese bank, and the objective is to predict if the customer will subscribe to an advanced offering. We will use Microsoft Azure to configure a cloud-based machine learning production model, deploy it, and consume it. Afterwards, we will create, publish, and consume a pipeline.

## Architectural Diagram
In this section, we will provide an architectual diagram of the project and give an introduction of each step. An architectural diagram is an image that helps visualize the flow of operations from start to finish.

![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/ArchitecturalDiagram.png?raw=true)

## Key Steps
Registered Dataset\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img01.PNG?raw=true)

Experiment Completed\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img02.PNG?raw=true)

Best Performing Model\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img03.PNG?raw=true)

Deploying the Best Model with Authentication\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/applicationinsightdisabled.PNG?raw=true)

Running Code to Enable Logging\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/applicationinsightenabled.PNG?raw=true)

Application Insights Enabled\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img04.PNG?raw=true)

Logs by logs.py Script\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img05.PNG?raw=true)

Swagger Documentation with API Contents\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img06%20-%20swagger.PNG?raw=true)

![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img07%20-%20swagger.PNG?raw=true)

![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img08%20-%20swagger.PNG?raw=true)

![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img09%20-%20swagger.PNG?raw=true)

![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img10%20-%20swagger.PNG?raw=true)

Model Consumption and JSON output\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img11.PNG?raw=true)

![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/endpoint-json-output.PNG?raw=true)

Benchmarking\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/benchmark1.PNG?raw=true)

![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/benchmark2.PNG?raw=true)

Pipeline Created\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img12%20-%20pipeline.PNG?raw=true)

Pipeline Endpoint\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img13%20-%20endpoint.PNG?raw=true)

Bankmarketing Dataset with AutoML Module\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img14%20-%20datasetwithautomlmodule.PNG?raw=true)

Published Pipeline Overview\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img14%20-%20publishedpipeline.PNG?raw=true)

Jupyter Notebook\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img15.PNG?raw=true)

ML Studio with Scheduled Run\
![alt text](https://github.com/riokorb/nd00333_AZMLND_C2/blob/master/img16.PNG?raw=true)


## Screen Recording
[Link to Screen Recording](https://drive.google.com/file/d/15Kepc-ELspkkJMJs-RpHteE58_3UWuiX/view?usp=sharing)

## Standout Suggestions
To derive opportunites for improvement, we could cross-reference other projects that have analyzed this dataset, and note down the best practices. 

One suggestion for the future would be to further clean the data as this dataset contains outliers which may influence the accuracy of our predictions. We can consider using a library such as Boruta, which is a feature selection wrapper algorithm that works well with classification problem, to identify features that can be dropped. Alternatively, we can also use the feature selection module available in Azure Machine Learning.

Another suggestion to improve the undertaking of this project would be to leverage batch inference pipeline capabilities. By including a ParallelRunStep to our pipeline via the Azure SDK, we can distribute the workload tasks into mini-batches, which should help to reduce the processing time. This will allow us to perform operations and review results more quickly.
