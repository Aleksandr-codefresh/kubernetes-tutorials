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
kubectl apply -f load-balancer.yaml
```
Check it:
```
minikube service load-balancer-dashboard -n kubernetes-dashboard
```
