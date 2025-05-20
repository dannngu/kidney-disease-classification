# kidney-disease-classification

Kidney disease classification with deep learning (MLflow & DVC)

## How to run?

### Steps:

1. clone the repository

```bash
https://github.com/dannngu/kidney-disease-classification.git
```

2.Create a venv environment after opening the respository
```bash
python -m venv venv
```

3.Activate the virtual venv environment
- osx/linux
```bash
source venv/bin/activate
```

- windows
```bash
.\venv\Scripts\activate
```


## MLflow

- [🔗MLfllow-Documentation](https://mlflow.org/docs/latest/index.html)


### dagshub setup
[🔗dagshub](https://dagshub.com/)

1. Create a `.env` file.

```
MLFLOW_TRACKING_URI=https://dagshub.com/your_username/kidney-disease-classification.mlflow
MLFLOW_TRACKING_USERNAME=your_username # ← DagsHub Username 
MLFLOW_TRACKING_PASSWORD=generated_token  # ← Token 

python script.py
```

2. or run this in your terminal
```bash
export MLFLOW_TRACKING_URI=https://dagshub.com/your_username/kidney-disease-classification.mlflow
export MLFLOW_TRACKING_USERNAME=your_username 
export MLFLOW_TRACKING_PASSWORD=generated_token
```




4.install the required dependencies
```bash
pip install -r requirements.txt
```