## Build the App by running the following commands

kubectl apply -f deployment.yaml

kubectl apply -f service.yaml

Note: Make sure you have installed Kubectl on your machine

## 🚀 How to Access the Application

Once the Kubernetes Service is up and running, you can access the app using the following steps:

### 1. Check the Service Details

Run the following command to see the NodePort:

kubectl get services

Look for the my-app-service (or the service name you used). It will show something like:

NAME             TYPE       CLUSTER-IP      EXTERNAL-IP   PORT(S)        AGE
my-app-service   NodePort   10.96.188.170   <none>        80:30007/TCP   1m

## 2. If You're Using Minikube
Use this command to open the app in your default web browser:

minikube service my-app-service

Once accessed:

The home page of the deployed app is now appeared on the web browser