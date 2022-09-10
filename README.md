Hello! This is a MLOps project based on the Kaggle Used Car Auction Prices dataset. The goal is to master the full lifetime cycle of ML model development. Project is fully created on the Yandex Cloud and covers:

- creation of a model (python, sklearn, xgboost)
- its tracking while training and validating (Yandex Cloud, s3-bucket, MLflow)
- orchestrating of retraining model and switching outdated model (Prefect)
- deployment of the best version as a web-service (docker, Flask) 
- Online and batch monitoring (Evidently, Prometeus, Graphana)
- Unit and Integration tests
- Using best practices with pytest, pylint, black, isort and pre-commit hooks

This guide contains all the instructions for reproducing the project, and the following links lead to a description of the main stages of creation.

Stage-0 Creation of cloud environment and preparation of original dataset 
Stage-1 Baseline models and pipelines 
Stage-2 Searching the best parameters with MLFlow tracking service 
Stage-3 Initial orchestrating with Prefect 
Stage-4 Deployment final model with Flask as a web-service 
Stage-5 Monitoring 
Stage-6 Tests

Deployment
insert correct values into .env
check ports for docker-compose is empty
    docker ps
        docker kill <container_id>
check ports for tunneling in VSCode is open
5001 for MLFlow
4200 for Prefect Orion
3000 for grafana
check for venv variables is setted after running run-venv.sh
