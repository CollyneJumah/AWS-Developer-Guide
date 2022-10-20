# Introduction
This guide provides all information on exam preps for AWS Cloud Developer.
## Domain 1: Deployment
### a. Deploy written code in AWS using existing CI/CD pipelines, processes, and patterns.

| Key Concepts| AWS Services | Link to resource |
| :---        |    :----:   |          ---: |
| Continuous Integration  | AWS CodeCommit | [click here](https://docs.aws.amazon.com/codecommit/index.html)  |
| Continuous Delivery  | AWS CodeBuild   | [click here](https://docs.aws.amazon.com/managedservices/latest/userguide/code-build.html) |
| Continuous Deployment  | AWS Code Pipeline  | [click here](https://docs.aws.amazon.com/codepipeline/latest/userguide/welcome.html) |
|    | AWS Code Deploy  | [click here](https://aws.amazon.com/codedeploy/) |

### b. Deploying application using Elastic Beanstalk
Key pointers include:
* Creating application using [Elastic Beanstalk](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/Welcome.html).
* How to manage its deployment.
* How to upgrade the deployment.
* How to remove it when its no longer needed.

### c. Prepare Application Deployment package to be deployed to AWS
> Understand how the `ebextensions` folder works and how to manage various types of deployments.
> Review 5-deployment policies offered by elastic beanstalks:
  * [Blue Green deployment](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/bluegreen-deployments.html)
  * [Prebaking vs Bootstrapping AMIs](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/prebaking-vs.-bootstrapping-amis.html)
  * [Rolling Deployments](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/rolling-deployments.html)
  * [In-Place deployments](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/in-place-deployments.html)
  * [Combining Deployment Services](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/combining-deployment-services.html)

### d. Depolyment Serverless Application
Learn by using [AWS Serverless Application Model (SAM)](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/what-is-sam.html)
> It can be used to define, test and deploy applications.

| Service| Description |
| :---        |    :----:   |  
| [API Gateway](https://aws.amazon.com/api-gateway/) | Know how to use API Gateway to manage different versions of your application 
|

## Domain 2: Security
> Do you understand data stewardship and how to protect the data as it move through the cloud using your application ?
### a. Making Authenticated calls to AWS Service
### b. Implement Encryption using AWS Service
### c. Implement Application authentication, and Authorization
> Primary AWS Services covered include:
* [AWS IAM (Identity & Access Management)]()
* [Amazon Cognito]()
* [AWS KMS]()
* [AWS Secret Manager]()

>Security topics
* [Identity Federation]()
* [Identity Provider]()
* [SAML]()

> Know how to secure access to data
> Limit access to those people and applications that need it
> How to scale access as needed

## Domain 3: Development with AWS Service
>Taking advantage of existing AWS Solutions, Serverless architectures, Distributed systems, asynchronous workflows and microservices
### 1. Write code for serverless applications
>You need to know the steps required in order to design & Implement code using the AWS Cloud.

>Know the differences between writing code on a monolithic platform and one that's serverless.

> Understanding psudocode to describe a Lambda Function.
* Understand how resource allocation works (How much memory has been allocated to a function)
* How do you incorporate custom libraries
* Effective use connection string to the databases
* Managing external dependencies


| Service| Description |
| :---        |    :----:   |  
| [AWS Lambda](https://aws.amazon.com/api-gateway/) | Serverless service 
| [AWS Step Function]() | An event driven orchestrator for serverless code | 

### 2. Translate Functional requirements into application design.
This process involves "AWS-fying " the problem: i.e Utilizing AWS services basing on the usecase.
> Understanding what's available to you as a developer inside the AWS ecosytem and being able to create AWS solution using those AWS Services and features

| Quetion topic | Service |
| :---        |    :----:   |  
| If Question asks: MySQL| [Amazon RDS]() 
| Web Server related question | [Amazon EC2]() |
| MySQL + Web Servers | [Elastic Beanstalk]()  |
### 3. Implement Application Design into application code.
### 4. Write code that interact with AWS Services by using API, SDKs & AWS CLI

| Service | Description |
| :---        |    :----:   |  
| [API Gateway]() |Use the API Gateway to ensure different versions of APIcan coexist without intefering with each other. This means understand how stage variables can be configured.

## Domain 4: Refactoring
### 1. Optimize Applications to best use AWS services & features
>Moving Existing applications into the cloud: Through Migration & Optimization.

| AWS Services and Featires |
| :---   |  
| [AWS Lambda]()
| [Amazon Cognito]()
| [Amazon SQS]()
| [Amazon SNS]()
| [Amazon S3]()
| [AWS Single Sign On]()
| [DynamoDB]()
| [Amazon ElastiCache]()

>Containers /Containerization: Understanding how containers work

>Integration with other AWS Services
- Containers have no built-in storage
- How to interact with services like: [DynamoDB]() and [S3]().
- usecases
- Security
- Cost Optimization
### 2. Migrating existing Application code to run on AWS 

## Domain 5: Monitoring & Troubleshooting
### a. Write code that can be monitored
### b. Perform Root cause analysis on faults found in testing and production

> Services include:
> - [Amazon CloudWatch]()
>   - A kitchen-sink type of service.
>   - Its a monitoring & Observability service from AWS that looks at infrasctructure.

> - [Amazon CloudTrail]()
>   - If you need to see what a Labda function did ? can be monitored using this service.

> - [AWS X-Ray]()
>   - A service that lets you follow code through a distributed system.
>   - It collects and records trace data to create a service map that can reveals latencies, HTTP statuses and Meta data that can be used for analysis.


### Additional Resources:
- [6 Essential courses for building Modern Applications on AWS
](https://training.resources.awscloud.com/modern-apps-traincert/infographic-6-essential-courses-for-building-modern-apps?sc_channel=sm&sc_campaign=AWS_Training_and_Certification&sc_publisher=LINKEDIN&sc_geo=GLOBAL&sc_outcome=adoption&trkCampaign=infographic&sc_content=TRAINCERT-300-ModernApps&trk=b2406c6f-24cc-4483-9f88-c586399b6edf&linkId=183783035)
- [Cloud Developer certification](https://training.resources.awscloud.com/get-certified-developer-associate)

NEXT ⏭️ [Compute in AWS](compute.md) 🖥️