# Overview

[![Python application test with Github Actions](https://github.com/opdo/azure-devops-pj2/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/opdo/azure-devops-pj2/actions/workflows/pythonapp.yml)

This is a sample Continuous Integration and Continuous Delivery using Azure technologies. Setting up Azure Pipelines to deploy the Application Code to Azure App Services. This repo will enable you to:

- Deploy the app in Azure CloudShell
- Deploy the app as an Azure App Service
- Load test

## Project Plan

* Trello Board: https://trello.com/b/Rxk23qNx/build-cd-cd-pipeline
* Project Plan: https://docs.google.com/spreadsheets/d/1VQ4gyWtM0k3aL63_SMB2_ZRmqv9MTRt4WB4Ck2yn2Bg/edit?usp=sharing

## Instructions

* Architectural Diagram

![Architectural Diagram](images/cd-diagram.png)

* Project running on Azure App Service

![Project running on Azure App Service](<images/04. Web app.png>)

* Project cloned into Azure Cloud Shell

`git clone git@github.com:opdo/azure-devops-pj2.git`

![Project cloned into Azure Cloud Shell](<images/01. Clone pj by ssh.png>)

* Output of a test run

`make all`

![Passing tests](<images/02. make all.png>)

* Output of GitHub Action build

![Output of GitHub Action build](<images/03. Git action.png>)

* Successful deploy of the project in Azure Pipelines.

![Running Azure App Service from Azure Pipelines automatic deployment](<images/08. Build CI CD.png>)

* Running Azure App Service from Azure Pipelines automatic deployment

![Output](<images/09. Website deploy success.png>)

* Successful prediction from deployed flask app in Azure Cloud Shell.  

![Prediction from deployed flask app](<images/05. make_predict_azure_app.png>)

* Output of streamed log files from deployed application

`az webapp log tail`

![az webapp log tail](<images/07. az webapp log tail.png>)

`https://vinhwebappudacitypj2.scm.azurewebsites.net/api/logs/docker`

![Web log](<images/06. Web log.png>)

* Load test

![Load test 1](<images/11. Load test 2.png>)

![Load test 2](<images/12. Load test 3.png>)

## Enhancements

- Configuration specific branch for specific environment, for example: develop branch for dev environment, release branch for production.
- Automatically trigger test after successful deployment
- Automatically deploy the maintenance page interface before deploying to the Production environment

## Demo 

Video demo: https://youtu.be/WX0qKXapKJA


