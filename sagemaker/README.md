# sklearn-pre-processor

This code is used for pre processing the raw data using AWS Sagemaker 

## Install the dependencies from requirements file

   - pip install -r requirements.txt
   
   The requirements file consists of all the required dependencies to be installed
   
## Make sure to add your credentials in the file ~/.aws/credentials

   [default]
   
   aws_access_key_id = 'your_access_key'
   
   aws_secret_access_key = 'your_secret_key'

## sklearn_preprocessing_local.ipynb

   This notebook consists of local execution of training the sklearn-pre-processor, batch transformation and real time
   transformation of the raw train data
  
## sklearn_preprocessing_cloud.ipynb

   This notebook consists of the training the pre processor, batch transformation and real time transformation
   run using 'ml.m4.xlarge' instance.
   
   - Endpoint-URL: https://runtime.sagemaker.us-east-2.amazonaws.com/endpoints/inference-pipeline-ep-2021-04-26-08-29-44/invocations
   
## dependencies.py 
  
   Any additional transformations(user-defined) can be added to this file if required.
 
## sklearn_entry_point.py

   This python script consists of the tranformations to be done on the raw data and also the functions required for training the sklearn-pre-processor

## Sequence of Steps listed in the notebook:

   - Import Libraries
   - Create SageMaker Scikit Estimator
   - Batch transform the training data
   - Real - Time Transformation of the training data : Create Endpoint
   - Make a request to the endpoint
   
## Training job created in AWS Sagemaker Console:

  <p>
  <img src="images/train_one.PNG" width="800">
  </p>
  
## Batch Transform job created in AWS Sagemaker Console:

  <p>
  <img src="images/batch_one.PNG" width="800">
  </p> 
  <p>
  <img src="images/batch_two.PNG" width="800">
  </p> 

## Endpoint created in AWS Sagemaker Console:

  <p>
  <img src="images/endpoint_two.PNG" width="800">
  </p>
  <p>
  <img src="images/endpoint_three.PNG" width="800">
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
  
  - EC2 Usage

  <p>
  <img src="images/usage_one.PNG" width="800">
  </p>

  - Sagemaker and S3 Usage
 
   <p>
  <img src="images/usage_two.PNG" width="800">
  </p>
