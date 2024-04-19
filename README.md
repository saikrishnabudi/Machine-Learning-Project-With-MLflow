# Machine-Learning-Project-with-MLflow

# End-To-End Machine Learning Project with MLflow

## Workflows

1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the app.py


# How to run?

### Steps:

Clone the repository

```bash
https://github.com/saikrishnabudi/Machine-Learning-Project-with-MLflow.git
```

### Step 01- Create a conda environment after opening the repository

```bash
conda create -n mlproject python=3.12 -y
```

```bash
conda activate mlproject
```

### Step 02- install the requirements
```bash
pip install -r requirements.txt
```

```bash
# Run the app.py
python app.py
```

Now,
open up the local host and port


## ML Flow

```bash
[Documentation](https://mlflow.org/docs/latest/index.html)
```

## cmd
```bash
- mlflow ui
```

### dagshub

```bash
[dagshub](https://dagshub.com/dashboard)

MLFLOW_TRACKING_URI=https://dagshub.com/saikrishnabudi/Machine-Learning-Project-with-MLflow.mlflow \
MLFLOW_TRACKING_USERNAME=saikrishnabudi \
MLFLOW_TRACKING_PASSWORD=3efda87a7165edecfd46af3e63ed69f73a2d4801 \
python script.py
```

Run this to expert as env variables:

```bash
export MLFLOW_TRACKING_URI=https://dagshub.com/saikrishnabudi/Machine-Learning-Project-with-MLflow.mlflow

export MLFLOW_TRACKING_USERNAME=saikrishnabudi

export MLFLOW_TRACKING_PASSWORD=3efda87a7165edecfd46af3e63ed69f73a2d4801
```
# AWS-CICD-Deployment-with-Github-Actions

### 1. Login to AWS console.

### 2. Create IAM user for deployment
```bash
#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess
```

# 3. Create ECR repo to store/save docker image
```bash
    - save the URI: 264413606393.dkr.ecr.ap-south-1.amazonaws.com/mlproject
```

# 4. Create EC2 machine (Ubuntu)

# 5. Open EC2 and Install docker in EC2 Machine:
```bash
sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker
```

# Docker Version
```bash
Docker version 26.0.2, build 3c863ff
```

# 6. Configure EC2 as self-hosted runner:
```bash
setting>actions>runner>new self hosted runner> choose os> then run command one by one
```

# 7. Setup github secrets:
```bash
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = ap-south-1

AWS_ECR_LOGIN_URI = demo>>  264413606393.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = mlproject
```