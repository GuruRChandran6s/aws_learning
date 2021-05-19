# xgboost-estimator

This code is used for training and deploying inbuilt XGBoost estimator using AWS Sagemaker 

## Create the environment from .yml file

   - conda env create -f env.yml
   
   The environment file consists of all the required dependencies to be installed

## Activate the environment created

   - conda activate sagemaker-env
   
## Make sure to add your credentials in the file ~/.aws/credentials

   [default]
   
   aws_access_key_id = 'your_access_key'
   
   aws_secret_access_key = 'your_secret_key'

## inbuilt-xgboost-model.ipynb

   This notebook consists of code for training and deploying inbuilt XGBoost estimator
   
## Sequence of Steps listed in the notebook:

   - Import Libraries
   - Create XG Boost Estimator
   - Create Hyperparameter Tuning Job
   - Associate the Tuning Job to Sagemaker Experiment
   - Select the Best model
   - Create Debugger Config using Best Model
   - Visualize feature importance and performance metrics
   - Endpoint creation
   - Make a request to the endpoint
   
   - Endpoint-URL: https://runtime.sagemaker.us-east-2.amazonaws.com/endpoints/xgboost-inference-pipeline-ep-2021-05-04-13-07-23/invocations

   
## Charts created using Sagemaker Experiments:

### x-axis: num_round, y-axis: train:rmse

  <p>
  <img src="images/chart_one.PNG" width="700">
  </p>
  
### x-axis: num_round, y-axis: validation:rmse

  <p>
  <img src="images/chart_two.PNG" width="700">
  </p>
  
### x-axis: gamma, y-axis: train:rmse

  <p>
  <img src="images/chart_three.PNG" width="700">
  </p>
  
### x-axis: gamma, y-axis: validation:rmse

  <p>
  <img src="images/chart_four.PNG" width="700">
  </p>
  
### x-axis: eta, y-axis: train:rmse

  <p>
  <img src="images/chart_five.PNG" width="700">
  </p>
  
### x-axis: eta, y-axis: validation:rmse

  <p>
  <img src="images/chart_six.PNG" width="700">
  </p>
  
### x-axis: max_depth, y-axis: train:rmse

  <p>
  <img src="images/chart_seven.PNG" width="700">
  </p>
  
### x-axis: max_depth, y-axis: validation:rmse

  <p>
  <img src="images/chart_eight.PNG" width="700">
  </p>
  
## Billing Report - grouped by service 

  The Billing Report can be viewed grouping by service 

  - Inbound Rules 
  <p>
  <img src="images/billing_service.PNG" width="800">
  </p>

## Billing Report - grouped by tags 

  The Billing Report can be viewed grouping by tags 

  - Inbound Rules 
  <p>
  <img src="images/billing_tags.PNG" width="800">
  </p>

## Free Tier Usage 
  
  - Data Transfer Usage

  <p>
  <img src="images/free_tier_one.PNG" width="800">
  </p>

  - Sagemaker and S3 Usage
 
   <p>
  <img src="images/free_tier_two.PNG" width="800">
  </p>
  
## HyperParameter Tuner jobs created in AWS Sagemaker Console:

  <p>
  <img src="images/tuning_job_one.PNG" width="800">
  </p> 
  <p>
  <img src="images/tuning_job_two.PNG" width="800">
  </p> 
  
  - Best training job
  
  <p>
  <img src="images/best_training_job.PNG" width="800">
  </p> 

## Stacked Force Plot

  <p>
  <img src="images/stacked_force_plot.PNG" width="700">
  </p> 
  
## Sagemaker Experiments created in AWS Sagemaker Notebook:

  <p>
  <img src="images/sagemaker_experiments.PNG" width="800">
  </p> 

## Endpoint created in AWS Sagemaker Console:

  <p>
  <img src="images/endpoint_one.PNG" width="800">
  </p>
  <p>
  <img src="images/endpoint_two.PNG" width="800">
  </p>


