Install minikube- https://minikube.sigs.k8s.io/docs/start/

Start minikube - `minikube start`  
Download kubectl - `minikube kubectl -- get po -A`  
Kubernetes Dashboard - `minikube dashboard`  
View cluster status `minikube status`  
Stop cluster `minikube stop`  
Delete cluster `minikube delete`  
View profile list `minikube profile list`  

```
$ minikube start --kubernetes-version=v1.23.3 \
  --driver=podman --profile minipod

$ minikube start --nodes=2 --kubernetes-version=v1.24.4 \
  --driver=docker --profile doubledocker

$ minikube start --driver=virtualbox --nodes=3 --disk-size=10g \
  --cpus=2 --memory=4g --kubernetes-version=v1.25.1 --cni=calico \
  --container-runtime=cri-o -p multivbox

$ minikube start --driver=docker --cpus=6 --memory=8g \
  --kubernetes-version="1.24.4" -p largedock

$ minikube start --driver=virtualbox -n 3 --container-runtime=containerd \
  --cni=calico -p minibox
```
