Run `minikube`:
```
minikube start
```
Enable ingress controller:
```
minikube addons enable ingress
```
Check ingress controller pod:
```
kubectl get pod -n ingress-nginx
```
Enable dashboard:
```
minikube addons enable dashboard
```
Check dashboard:
```
kubectl get all -n kubernetes-dashboard
```
Apply ingress rules:
```
kubectl apply -f dashboard-ingress.yaml
```
Check it and wait for IP address:
```
kubectl get ingress -n kubernetes-dashboard --wait
```
Define IP mapping in the `/etc/hosts`:
```
sudo nano /etc/hosts
```
For example:
`192.168.64.5 dashboard.io`
