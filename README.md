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
kubectl get configmap -o yaml (namespace info)
kubectl apply -f mysql-configmap.yaml --namespace=my-namespace (or define inse the metadata attribute in yaml files.)
minikube service go-backend-service --url (for service url)
````
## Kubernetes Namespaces Notes
````
1-) Structure components
2-) Avoid conflicts between teams
3-) Share services between different environments
4-) Access and Resource Limits on namespace level
5-) each ns must define own configmap and secrets
6-) accessing service in another namespace: mysql-service.namespace 

by default components are created in a default ns

kubectx -> set default name space and avoid adding -n on every command.

````
## Kubernetes Ingress Notes
````
minikube addons enable ingress
(k8s ngnix ingress controller)

kubectl get pod -n kube-system --> nginx ingresses
````