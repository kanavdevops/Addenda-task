# Addenda-task
Please run the below commands

#Mongo configurations
kubectl create -f mongo-db-secret.yaml
kubectl create -f mongo-pv.yaml
kubectl create -f mongo-pvc.yaml
kubectl create -f mongo-deployment.yaml
kubectl create -f mongo-test-svc.yaml


#Nodejs Configurations
kubectl create -f node-cm.yaml
kubectl create -f node-api-deployment.yaml
kubectl create -f node-api-svc.yaml

