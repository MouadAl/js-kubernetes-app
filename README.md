# Developping using Docker-Kubernetes (Part2)


## What it does:

this is the second part where I will deploy the application  and MongoDB in Kubernetes cluster


## What I have learned:
<ul>
  <li>Setting up a k8s cluster with minikube</li>
  <li>Deployment && Services</li>
  <li>Config-map && Secret</li>
</ul>

## How to run ?

 Step1: Start minikube <br/>
  ` minikube start --driver=docker `<br/>
  
 Step 2: Execute the folowwing commands in order: <br/>
``` 
kubectl apply -f mongo-secret.yml
kubectl apply -f mongo-configmap.yml 
kubectl apply -f mongo.yml
kubectl apply -f webapp.yml
```
Step 3: Commands to get informations about your cluster <br/>
``` 
kubectl get pod
kubectl get pod -o wide
kubectl get service
kubectl get secret
kubectl get all 
```






