# Hummingbird Command Job Example

View an example of the run, its environment, and outputs here:https://ml.azure.com/experiments/id/f2ff31b4-44f9-4d3f-9a65-b78e80056c57/runs/green_caravan_k4ptbq6yzz?wsid=/subscriptions/ea4faa5b-5e44-4236-91f6-5483d5b17d14/resourceGroups/t-xiechloe/providers/Microsoft.MachineLearningServices/workspaces/t-xiechloe&tid=72f988bf-86f1-41af-91ab-2d7cd011db47 <br>
Example of Hummingbird, MLflow, and Azure Machine Learning integration. 
We create an Sklearn model, log it with MLflow, convert it to Pytorch, and log that through the Azure CLI as a command job.

1. Install and set up the CLI: https://docs.microsoft.com/en-us/azure/machine-learning/how-to-configure-cli?tabs=public
2. Follow this set up on how to train: https://docs.microsoft.com/en-us/azure/machine-learning/how-to-train-cli 
3. Set up the environment Dockerfile to have mlflow, azureml-mlflow, azureml-core
4. Log in to AZ CLI <br>
`az login --scope https://management.azure.com/.default`
5. Run the script <br>
`az ml job create -f job_blog.yml  --web`
