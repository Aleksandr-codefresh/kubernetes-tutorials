Run `minikube`:
```
minikube start
```
Enable dashboard:
```
minikube addons enable dashboard
```
Check dashboard:
```
kubectl get all -n kubernetes-dashboard
```
Apply load balancer:
```
kubectl apply -f node-port.yaml
```
Check it:
```
minikube service node-port-dashboard -n kubernetes-dashboard
```
