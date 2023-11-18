### ref. https://www.babelcoder.com/blog/articles/skaffold

## install kube mini 
https://devopscube.com/minikube-mac/

brew install qemu

brew install socket_vmnet
brew tap homebrew/services
HOMEBREW=$(which brew) && sudo ${HOMEBREW} services start socket_vmnet

brew install minikube

minikube start --driver qemu --network socket_vmnet

## install skaffold

brew install skaffold
sudo port install skaffold

## start system

minikube start
## minikube status
## kubectl get nodes
## kubectl cluster-info
## minikube dashboard
## kubectl get all

## kubectl delete service/node-app  
## kubectl delete deployment.apps/node-app 
## kubectl get pods -w

##  minikube stop

eval $(minikube docker-env)
## eval $(minikube docker-env -u)
## echo $DOCKER_TLS_VERIFY $DOCKER_HOST $DOCKER_CERT_PATH

## docker image prune -a
## Remove all unused images, not just dangling ones. Add -f option to force.

docker images

## pull code frome git


npm install express


# forward port to local

skaffold dev

minikube service node-app


## ################################################

