This project demonstrates a simple, fully serverless web application built on top of AWS services. The backend is powered by AWS Lambda, which handles the application logic, API Gateway for RESTful API access, and DynamoDB for fast, scalable NoSQL storage. Optionally, the frontend can be hosted using Amazon S3 and distributed via CloudFront.
ARCHITECTURE OVERVIEW
Client (Browser / Frontend)
        |
        v
   Amazon API Gateway
        |
        v
   AWS Lambda Functions
        |
        v
   Amazon DynamoDB (NoSQL Database)

Tech Stack
AWS Lambda – Serverless compute for backend logic.

Amazon API Gateway – REST API exposure to clients.

Amazon DynamoDB – Managed NoSQL database for storage.

AWS IAM – Role-based access control.

(Optional) Amazon S3 + CloudFront – Static frontend hosting.

How to Deploy
Clone the Repository:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Setup Lambda Function:

Create a Lambda function using provided lambda_function.py.

Assign an IAM role with DynamoDB permissions.

Create DynamoDB Table:

Table Name: users

Primary Key: userId (String)

Configure API Gateway:

Setup HTTP API Gateway.

Link methods to Lambda functions.


