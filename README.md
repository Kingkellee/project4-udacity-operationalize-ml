**This Badge showcase my ability to operationalize production microservices.**

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Kingkellee/project4-udacity-operationalize-ml/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Kingkellee/project4-udacity-operationalize-ml/tree/master)

## Project Overview

This project sougth to test the skills acquired in the cource Microservices at Scale using AWS & Kubernetes by Udacity Cloud DevOps Nanodegree.

A pre-trained `sklearn` model to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on was given to operationalize a Machine Learning Microservice API. More about the data, which was initially taken from Kaggle can bee found here [the data source site](https://www.kaggle.com/c/boston-housing).

### Project Tasks

The aim of this project is to operationalize a working machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project my ability to complete the following task was tested:

- Test project code using linting
- Complete a Dockerfile to containerize an application
- Deploy a containerized application using Docker and make a prediction
- Improve log statements in the source code for the application
- Configure Kubernetes and create a Kubernetes cluster
- Deploy a container using Kubernetes and make a prediction
- Upload a complete Github repo with CircleCI to indicate that code has been tested

You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

---

### Running This App

## 1. Setup the Environment

- Create a virtualenv with Python 3.7 and activate it.
  - This project runs well on Python 3.7, so you should have Python 3.7 available on your host.

```bash
python3 -m pip install --user virtualenv
# Check the Python path using `which python3`
# Use this command to enable Virtual Env run on Pytghon 3.7:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
#use this command to activate Virtual Env
source .devops/bin/activate
```

- Run `make install`

```bash
 #To install the necessary dependencies
 make install
```

- Install Hadolint

# To Install Hadolint on Linux

```bash
 # Step 1.
 sudo apt update
```

```bash
 # Step 2.
 sudo apt-get install build-essential
```

```bash
 # Step 3 run the Homebrew installation script
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```bash
 # Step 4 add homebrew to path
 eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```

```bash
 # Step 5. Optional
 brew install gcc
```

```bash
 # Step 6. Install Hadolint
 brew install hadolint
```

```bash
 # Step 7. Lint Dockerfile
 hadolint Dockerfile
```

## 2. Docker Steps: `./run_docker.sh`

```bash
 #To run Docker Container
 ./run_docker.sh
```

## 3. Upload to Docker Hub: `./upload_docker.sh`

```bash
 #To upload to docker hub, run
 ./upload_docker.sh
```

### 4. Kubernetes Steps: `./run_kubernetes.sh`

```bash
 #To deploy to kubernetes, run
 ./run_kubernetes.sh
```
