# AWS SageMaker Deployment Project

Web Application complete with a RNN trained for Sentiment Analysis and Web API built, trained, and deployed through AWS SageMaker. Final Udacity Deep Learning Nanodegree project.

# User Function
The application provides a sentiment analysis solution for users - trained on the IMDB Large Movie review dataset.

Users input a review or sentence of his or her choosing into the web application and will receive whether or not the input's sentiment is Good or Bad.

# High-Level Data Flow
1. User inputs Review into Web App
2. Review is sent to AWS Gateway API
3. AWS Gateway API Sends the Review to the Preprocessing Lambda Function
4. Lambda Function preprocesses the data then invokes the Deployed Model's Endpoint for inference
5. Model Returns predicted sentiment to Lambda Function
6. Lambda function returns result to AWS Gateway API
7. Result returned to Web App to User

<img src="./Web App Diagram.svg">