# KUBERNETES NGINX COMMANDS

## 1. Check Kubernetes

minikube start

# Starts the local Kubernetes cluster

kubectl cluster-info

# Displays cluster information

kubectl get nodes

# Lists cluster nodes

## 2. Create Nginx Deployment

kubectl create deployment nginx --image=nginx

# Creates an Nginx deployment

kubectl get deployments

# Lists deployments

kubectl get pods

# Lists running pods

## 3. Expose Deployment

kubectl expose deployment nginx --type=NodePort --port=80

# Exposes Nginx through a NodePort service

kubectl get services

# Lists services

minikube service nginx

# Opens the Nginx service in a browser

## 4. Scale Deployment

kubectl scale deployment nginx --replicas=3

# Scales Nginx to 3 replicas

kubectl get pods

# Checks the three pods

kubectl scale deployment nginx --replicas=5

# Scales Nginx to 5 replicas

## 5. Check Deployment Details

kubectl describe deployment nginx

# Displays deployment details

kubectl get all

# Displays deployments, pods and services

## 6. Delete Resources

kubectl delete service nginx

# Deletes the Nginx service

kubectl delete deployment nginx

# Deletes the Nginx deployment

minikube stop

# Stops the Kubernetes cluster
