# Hummingbird Command Job Example

Example of Hummingbird, MLflow, and Azure Machine Learning integration. 
We create an Sklearn model, log it with MLflow, convert it to Pytorch, and log that through the Azure CLI as a command job.

1. Install and set up the CLI: https://docs.microsoft.com/en-us/azure/machine-learning/how-to-configure-cli?tabs=public
2. Follow this set up on how to train: https://docs.microsoft.com/en-us/azure/machine-learning/how-to-train-cli 
3. Log in to AZ CLI <br>
`az login --scope https://management.azure.com/.default`
4. Run the script <br>
`az ml job create -f job_blog.yml  --web`
