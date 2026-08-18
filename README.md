# Amazon-ECS-Project

Write-up of project following the ECS workshop listed here

https://catalog.us-east-1.prod.workshops.aws/workshops/8c9036a7-7564-434c-b558-3588754e21f5/en-US

Will build and deploy a containerized web application that displays a cat picture. 

Will implement container observability tools, load testing and monitoring.

Successful completion of this workshop will give us a working example of:

    Amazon Elastic Container Service (ECS)
    Amazon Elastic Container Resistry (ECR)
    AWS Fargate
    Amazon CloudWatch
    Auto Scaling
    AWS Identity and Access Management (IAM)
    Amazon CloudFormation
    Amazon EC2
    Amazon Application Load Balancer (ALB)

# Configuring-and-Setup

Signed up for free tier AWS account

Created IAM user and configured according to instructions.

Download AWS CloudFormation template from workshop, and then uploaded it to cloudformation console.

Set up IDE environment using VSCode


# Amazon ECR

Created ECR repositories for web, cats, and dogs.

Build docker images for web, cats, and dogs

Tag and push container images to repositories

# Amazon ECS

ECS Cluster is a logical grouping of tasks or services
 
Go to EC2 Page and create and configure security group

Create and configure ECS Cluster Security Group

Create ECS Cluster

Create web, cats, dogs task definition and configure

Create and configure load balancer and web, cats, dogs service

# Monitoring

Use Amazon CloudWatch Container Insights to visualize log data from cats service

# Auto Scaling

Use ECS CloudWatch metrics to scale cats and dogs service/cluster

Configure service and cluster auto scale

# CI/CD Pipeline

Will create a CI/CD pipeline using AWS code services so that there is a AWS Code commit repository
that builds a new contianer image and deploys it to amazon ecs whenever the source is modified

Configure and go to AWS code pipeline to create a pipeline.

Modified code of dogs service to verify pipeline is working.

