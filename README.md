## MLFOW experiments

import dagshub
dagshub.init(repo_owner='kraj2003', repo_name='MLFLOW_project', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

mlflow.set_tracking_uri('https://dagshub.com/<DagsHub-user-name>/<repository-name>.mlflow')
https://dagshub.com/kraj2003/MLFLOW_project.mlflow