# Building-an-EKS-cluster-using-Terraform-and-Deploying-a-simple-Hello World application hosted on EKS cluster.
This repository contains all the relevant Terrform and CloudFormation codes that you need to deploy an EKS Cluster on AWS and also Deployment,Service,ConfigMaps and other Kubernetes objects definition files that is required to host an application on Kubernetes.I have tried to automate this as much as I can & avoid manual deployments.

Provisioning of initial components like EKS VPC has been done using CloudFormation and the actual EKS Cluster with Cluster IAM Roles etc has been using Terraform codes.

Provisioned a simple Hello World application as part of Kubernetes Deployment which runs on port 80 and have also configured a service.You can access the application by pasting the hostname of the service(a384a74b37062417e9cb0a23bac6ef0c-1050431180.eu-central-1.elb.amazonaws.com) in a browser of your choice.

Set-up Prometheus as the monitoring solution and integrated it with Alert Manager to get an email alert if the Memory of the POD goes beyond 10%.

Injected a Kubernetes Secret into the Deployment definition file of the application.

All the relevant codes to deploy the VPC,EKS Cluster(.tf files) and YAML files to deploy the application,prometheus,alert manager are present.

Output & Screenshots.docx file gives you the output & screenshots of the actual deployment which I have done.

Output of EKS Deployment using Terraform.txt file contains the output of EKS deployment using Terraform which will give you an understanding on how can we deploy the tf files.

Creating the VPC for EKS & post steps.txt file contains the steps of creating a VPC using CF template pre and post steps.

