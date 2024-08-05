
kubectl get pods
<br>
kubectl get deployment
<br>
kubectl create deployment nginx-depl --image=nginx
<br>
kubectl get replicaset
<br>
kubectl edit deployment nginx-depl
<br>
kubectl logs "pod name"
<br>
kubectl describe pod "pod name"
<br>
kubectl exec -it "pod name" -- bin/bash
<br>
kubectl delete deployment "deployment name"
<br>
kubectl apply -f config-file.yaml
<br>
kubectl get deployment nginx-deployment2 -o yaml
