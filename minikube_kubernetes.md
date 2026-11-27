in powershell:
minikube start

in another powershell:
kubectl create deployment mynginx --image=nginx
kubectl get deployments
kubectl expose deployment mynginx --type=NodePort --port=80 --target-port=80
kubectl scale deployment mynginx --replicas=4
kubectl get deployments
kubectl get pods
kubectl port-forward svc/mynginx 8081:80

open browser and check
