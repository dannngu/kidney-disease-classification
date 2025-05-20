# kidney-disease-classification

Kidney disease classification with deep learning (MLflow & DVC)

### How to run?

>[!NOTE]
> Since the model uses VGG16 and Python 3.10.5, `tensorflow==2.12.0` and `mlflow==2.2.2` is required for proper execution.

### Steps:

1. clone the repository

```bash
https://github.com/dannngu/kidney-disease-classification.git
```

2. Create a venv environment after opening the respository
```bash
python -m venv venv
```

3. Activate the virtual venv environment
- osx/linux
```bash
source venv/bin/activate
```


- windows
>[!IMPORTANT]
>On Windows, it is recommended to use `Anaconda3` to create a **virtual environment**, as it better handles dependencies like `pyarrow`.
```bash
conda create --name my_env python=3.10
conda activate my_env
```
>[!TIP]
> Use `Anaconda PowerShell` to execute `pip install -r requirments.txt` to make sure you are installing the dependencies in the desire vitural environment.


4. install the required dependencies
```bash
pip install -r requirements.txt
```


### MLflow

- [🔗MLfllow-Documentation](https://mlflow.org/docs/latest/index.html)


### DagsHub setup
- [🔗dagshub](https://dagshub.com/)

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

### DVC Commands to Run
- [🔗DVC](https://dvc.org/)
- 
1. Initialize DVC
```bash
dvc init
```
2. Run the DVC Pipeline
```bash
dvc repro
```
3. Display the Full DVC Pipeline Graph
```bash
dvg dag
```


