[Blog](https://matthewpalmer.net/kubernetes-app-developer/articles/kubernetes-ingress-guide-nginx-example.html)

1. Start minikube `minikube start`;
2. Enable ingress controller `minikube addons enable ingress`;
3. Apply all resources;
4. Get cluster ip `minikube ip` or `kubectl cluster-info`
5. Go to `http://CLUSTER_IP/apple` or `http://CLUSTER_IP/banana`