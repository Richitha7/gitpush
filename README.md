# gitpush
##DEPLOYING AND SCALING APPLICATIONS USING MINIKUBE
 `1.minikube start`
 `2.kubectl create deployment mynginx --image=nginx`
 
 `3.kubectl get deployments`
 
 `4.kubectl expose deployment mynginx --type=NodePort --port=80 --target-port=80`
 
 `5.kubectl scale deployment mynginx --replicas=4`
 
 `6.kubectl get pods`
 
`7. kubectl port-forward svc/mynginx 8081:80`
( in another powershell (minikube dashboard))
 `8.kubectl delete deployment mynginx`

###NAGIOS
`1.docker pull jasonrivers/nagios:latest`

`2.docker run --name selab -p 8888:80 jasonrivers/nagios:latest`

`3.docker ps`

`4.docker stop selab`

###DOCKER COMPOSE
(docker-compose.yaml)
cd C:\
`docker-compose up -d`
(localhost:8000)

### MODIFY AND PUSH DOCKER IMAGE
`1.docker pull ubuntu`
`2.docker run -it --name newubuntu -d ubuntu`
`3.docker ps`
`4.docker exec -it (container id) bash`
`5.git --version`
`6.apt update`
`7.apt install git -y`
`8.git --version`
`9.exit`
`10.docker stop (c-id)`
`11.docker commit (c-id) richitha7/newubuntu2025`
`12.docker login`
`13.docker push richitha7/newubuntu2025`

