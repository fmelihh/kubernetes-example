## Kubectl Example Commands
````
kubectl get pods
kubectl get deployment
kubectl create deployment nginx-depl --image=nginx
kubectl get replicaset
kubectl edit deployment nginx-depl
kubectl logs "pod name"
kubectl describe pod "pod name"
kubectl exec -it "pod name" -- bin/bash
kubectl delete deployment "deployment name"
kubectl apply -f config-file.yaml
kubectl get deployment nginx-deployment2 -o yaml
kubectl delete --all <pods,deployments,services.. etc>
kubectl get secret
kubectl get pod --watch
kubectl get pod -o wide
kubectl get all | grep mongodb
minikube service mongo-express-service
kubectl get namespace
kubectl create namespace my-namespace
````
## Kubernetes Namespaces Notes
````
1-) Structure components
2-) Avoid conflicts between teams
3-) Share services between different environments
4-) Access and Resource Limits on namespace level
````
