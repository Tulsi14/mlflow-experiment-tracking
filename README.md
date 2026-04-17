# Wine Quality Prediction with MLflow

A simple machine learning project demonstrating how to train an ElasticNet regression model to predict the quality of wine based on its physicochemical properties. The project uses **MLflow** for experiment tracking, model logging, and performance evaluation.

## Features
* **Machine Learning**: Predicts wine quality using `scikit-learn`'s ElasticNet model.
* **Experiment Tracking**: Logs hyperparameters (`alpha`, `l1_ratio`) and evaluation metrics (`RMSE`, `MAE`, `R2`) using MLflow.
* **Model Registry**: Automatically saves the trained model along with its input/output signature.

## Dataset
The dataset used in this project is the **Wine Quality Dataset** from the UCI Machine Learning Repository. It is automatically downloaded during script execution.

## Prerequisites
Make sure you have Python 3 installed. Install the required dependencies using:

```bash
pip install pandas numpy scikit-learn mlflow skops
```
# How to Run
## Clone the repository:

```Bash
git clone [https://github.com/Tulsi14/mlflow-experiment-tracking.git](https://github.com/Tulsi14/mlflow-experiment-tracking.git)
cd mlflow-experiment-tracking
```

## Run the training script:
### You can run the script with default parameters:

```Bash
python main.py
```
### Or, you can provide custom parameters for alpha and l1_ratio:

```Bash
python main.py 0.5 0.8
```

# Viewing the MLflow Dashboard
### To view your tracked experiments, metrics, and models, start the MLflow UI:

```Bash
mlflow ui
```
1. Open your web browser and go to http://127.0.0.1:5000.

2. On the top left corner, ensure you switch the toggle from GenAI to Model training.

3. Click on the Default experiment in the sidebar to see your training runs.
