# quarkus-test Deployment

# quarkus-test Project

This project uses Quarkus, the Supersonic Subatomic Java Framework.

If you want to learn more about Quarkus, please visit its website: https://quarkus.io/ .

## Running the application in minikube kubernetes cluster

You can run your application in a minikube kubernetes cluster using:

```shell script
#Start the master node
minikube start --driver docker
#Apply the cluster configuration
kubectl apply -f kubernetes/
#Expose the backend service to localhost
minikube service quarkus-backend-service
```

## Running the application in fully dockerized mode

You can run your application in a local docker network:

```shell script
docker-compose -p quarkus-test -f docker-compose/<docker-compose-file> up --build
```
