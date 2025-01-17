# gitpush
#DEPLOYING AND SCALING APPLICATIONS USING MINIKUBE
 minikube start
 kubectl create deployment mynginx --image=nginx
 kubectl get deployments
 kubectl expose deployment mynginx --type=NodePort --port=80 --target-port=80
 kubectl scale deployment mynginx --replicas=4
 kubectl get pods
 kubectl port-forward svc/mynginx 8081:80
( in another powershell (minikube dashboard))
 kubectl delete deployment myngnix
