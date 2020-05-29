# AutoML-MLOps
It is found that 60–90% of Machine Learning and AI models fail in real-world reason is a lot of manual work for the data scientist to changer values which are known as parameters in the technical world. Here comes the big concept to discuss for automation in AI world i.e. Hyper Parameters which can be classified as model hyperparameters, that cannot be inferred while fitting the machine to the training set because they refer to the model selection task, or algorithm hyperparameters, that in principle have no influence on the performance of the model but affect the speed and quality of the learning process. An example of a model hyperparameter is the topology and size of a neural network. Examples of algorithm hyperparameters are learning rate and mini-batch size. Today, I’m gonna show you my project in which I have successfully integrated my Deep Learning model on Jenkins using Docker image created by me for running a container where one can easily achieve model training using Docker OS. Below is the summary of Jobs which we are going to build over Jenkins for the project:

## Create a container image that has Python3, tensorflow, Keras, Pandas, Sci-kit Learn and NumPy installed using Dockerfile.

## When we launch this image, It should automatically start training the model in the container.

## Create a Job chain of job1, job2, job3, job4 and job5 using build pipeline plugin in Jenkins

## Job1: Pull the Github repo automatically when some developers push the repo to Github.

## Job2: By looking at the code or program file, Jenkins should automatically start the respective machine learning software installed interpreter install image container to deploy code and start training( eg. If code uses CNN, then Jenkins should start the container that has already installed all the software required for the CNN processing).

## Job3: Train your model and predict accuracy or metrics.

## Job4: If metrics accuracy is less than 99%{Desired Accuracy}, then tweak the machine learning model architecture.

## Job5: Retrain the model until desired accuracy achieved and also notify developer by e-mail that the best model is being created.

## Create One extra job job6 for monitor: If the container where the app is running fails due to any reason then this job should automatically start the container again from where the last trained model left.

# Blog
[BLog for AutoML](https://medium.com/@ghumare64/getting-ai-ml-and-devops-working-better-together-for-automation-e6de4b588231)

# Author
[Rohit Ghumare](https://github.com/rohitg00)
