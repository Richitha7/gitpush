# gitpush
##DEPLOYING AND SCALING APPLICATIONS USING MINIKUBE
 ###1.minikube start
 ###2.kubectl create deployment mynginx --image=nginx
 **3.kubectl get deployments**
 **4.kubectl expose deployment mynginx --type=NodePort --port=80 --target-port=80**
 5.kubectl scale deployment mynginx --replicas=4
 6.kubectl get pods
7. kubectl port-forward svc/mynginx 8081:80
( in another powershell (minikube dashboard))
 8.kubectl delete deployment mynginx

###NAGIOS
docker pull jasonrivers/nagios:latest
docker run --name selab -p 8888:80 jasonrivers/nagios:latest
docker ps
docker stop selab

###DOCKER COMPOSE
(docker-compose.yaml)
cd C:\
docker-compose up -d
(localhost:8000)

### MODIFY AND PUSH DOCKER IMAGE
docker pull ubuntu
docker run -it --name newubuntu -d ubuntu
docker ps
docker exec -it (container id) bash
git --version
apt update
apt install git -y
git --version
exit
docker stop (c-id)
docker commit (c-id) richitha7/newubuntu2025
docker login
docker push richitha7/newubuntu2025

