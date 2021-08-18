# SageMaker

* first let's create a notebook instance with notebook jupyter
* Prepare the data
* Train the model to learn from the data
* Deploy the model
* Evaluate model performance

## Initially create a notebook notes in SageMaker, creating a new function in IAM.
![sagemaker](https://user-images.githubusercontent.com/78814110/129970746-6a69a038-4335-41c6-a9d9-6d281c6faf0f.jpg)

## We will create our Datalake in The Following S3.
![s3](https://user-images.githubusercontent.com/78814110/129970857-71a058fd-2100-47ec-b627-03100326788b.jpg)

The link to the training raw file is on that link.
(https://d1.awsstatic.com/tmt/build-train-deploy-machine-learning-model-sagemaker/bank_clean.27f01fbbdf43271788427f3682996ae29ceca05d.csv)

70% of customers will be used during the training loop. The remaining 30% will be used to evaluate model performance.
After we use the pandas library to handle this data and concatenate and send it to our Bucket S3.
We will generate an EC2 instance to perform this training, for this will require a stronger virtual machine.
After we put our model to perform the training, this may take a few minutes.

![cloudwatch](https://user-images.githubusercontent.com/78814110/129971808-12e7f903-bfa8-48f1-a465-3ceb23373d2a.jpg)


## Now let's deploy this model on an endpoint and run the to perform predictions
## Let's take our data and load it into an array and evaluate the performance of the model.

With the data generated if it were the case we could use this analysis to make a specific Marketing for that group of customers.
Done that we can delete our services on AWS because it brings savings.


