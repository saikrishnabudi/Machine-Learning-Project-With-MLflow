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
```bash
open up the local host and port
```

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


