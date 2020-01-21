# SpringBoot and Elastic Search Example on Google Compute Engine

## Install GKE with Elastic Search
This section involves a couple of steps: install GKE on a supported IaaS, install Elastic Search on the deployed Kubernetes cluster and load the Location data. We will use a sample dataset in this case, but you can load any other Positional data of your choice and have it display on the map accordingly. This is a good website to download Location data based on your specific customer's need. 

[Location Data Source](https://www.aggdata.com)

[Deploying Elastic Search on Kubernetes](https://github.com/kubernetes/examples/tree/master/staging/elasticsearch)

## Install the Spring Boot application on PAS
This is a sample SpringBoot application that performs Geo Bounded queries against an Elastic Search instance and plots the data on a map interactively. This application can be run on a workstation or in a cloud environment such as GKE. In this example, I will show how to deploy the application on a running GKE instance. 

## Testing the application

1. Navigate to the route thats created for the application.

<img src="https://github.com/gvijayar/springboot-elasticsearch/blob/master/docs/default.jpg" width="80%"/>

2. You can now interact with the map by zooming in/out or shifting the focus. It should execute a new Geo Positional query against GKE and repaint the map.

<img src="https://github.com/gvijayar/springboot-elasticsearch/blob/master/docs/zoom.jpg" width="80%"/>
