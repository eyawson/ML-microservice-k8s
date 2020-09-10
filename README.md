# Operationalize a Machine Learning Microservice API

[![eyawson](https://circleci.com/gh/eyawson/ML-microservice-k8s.svg?style=svg)](https://app.circleci.com/pipelines/github/eyawson/ML-microservice-k8s)

## Project Overview

In this project, I operationalized a Machine Learning Microservice API.

## Background

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Running the application

1. Run standalone:  `python app.py` and then use `./make_prediction.sh` for a prediction
2. Run in Docker:  `./run_docker.sh` and then use `./make_prediction.sh` for a prediction
3. Run in Kubernetes:  `./run_kubernetes.sh` and then use `./make_prediction.sh` for a prediction

### Project Tasks

The project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project I:

* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

**The final implementation of the project will showcased my abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Files in repo

* Makefile for build automation
* scripts to automate repeatable tasks and set up kubernetes
* Dockerfile to containerize the application
* CircleCI config file CI purposes
* App.py to run the prediction application
* Data for app in the model_data folder
