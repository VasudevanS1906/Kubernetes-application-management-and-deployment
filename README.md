# Kubernetes-Application-Management-and-Deployment
Deployed and managed a containerized Nginx web application on a Kubernetes cluster, utilizing manifests to create Deployments, Services, and ConfigMaps. Scaled the application from 2 to 4 replicas, performed rolling updates with zero downtime, and troubleshot issues using kubectl commands, demonstrating proficiency in essential Kubernetes concepts and operations.

# Prerequisites

Before getting started, make sure you have the following prerequisites installed:

1.Git

2.Kubernetes cluster (local or remote)

# Getting Started

To get started with this project, follow these steps:

Clone the repository:

      git clone https://github.com/VasudevanS1906/kubernetes-application-management-and-deployment.git

Change to the project directory:

      cd kubernetes-web-app-deployment

# Usage

This project provides hands-on experience with deploying and managing a web application using Kubernetes. Here's how you can use it:

1. Set up a Kubernetes Cluster

Set up a Kubernetes cluster locally or on a cloud platform.

2. Deploy the Application

To deploy the web application, run the following command:

      kubectl apply -f .
This command will apply all the necessary resources (Deployment, Service, etc.) to the cluster.

3. Scale the Application

You can scale the application by modifying the number of replicas in the Deployment. For example:

      kubectl scale deployment/app --replicas=5

4. Access the Application
Once the application is deployed, you can access it by exposing the Service. 

      kubectl port-forward service/app 8080:80

5. Monitoring and Troubleshooting

For monitoring and troubleshooting purposes, you can use various Kubernetes commands and tools, such as kubectl get, kubectl describe, kubectl logs, and kubectl exec.

6. Cleanup

When you're done, you can delete the resources created by this project by running the following command:

      kubectl delete service,deployment app
