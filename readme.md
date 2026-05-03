# Kubernetes courses

## Launch services

1. Launch docker
2. Install minikube :  ```curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-amd64```
```sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64```
3. Launch minikube : ```minikube start --extra-config="apiserver.cors-allowed-origins=['http://boot.dev']"```
4. create dashboard : ```minikube dashboard --port=63840``` -> (http://localhost:63840/)
5. Clone image docker webchat : ```kubectl create deployment synergychat-web --image=docker.io/bootdotdev/synergychat-web:latest```
6. install Envoy Gateway : ```kubectl apply --server-side -f https://github.com/envoyproxy/gateway/releases/download/v1.5.1/install.yaml```


## For submit commands to bootdev

1. ```kubectl proxy```
2. ```minikube tunnel -c```