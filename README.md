# Addenda-task
Please run the below commands in the order mentioned below

#Mongo configurations

<kubectl create -f mongo-db-secret.yaml>
  
<kubectl create -f mongo-pv.yaml>  # where ever the pod launches cd /mongo/data for the pv 
  
<kubectl create -f mongo-pvc.yaml>
  
<kubectl create -f mongo-deployment.yaml>
  
<kubectl create -f mongo-test-svc.yaml>


#Nodejs Configurations

<kubectl create -f node-cm.yaml>
  
<kubectl create -f node-api-deployment.yaml>
  
<kubectl create -f node-api-svc.yaml>


#Curl pod
kubectl run --generator=run-pod/v1 curl --image=tutum/curl --command -- sleep 500000

