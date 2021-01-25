# Prerequisites

First, install a nice curl client : [httpie](https://httpie.org/)

`sudo apt-get -y install httpie`{{execute}}



, then setup Kubernetes environment.

Start the cluster:


`minikube start --wait=false`{{execute}}

Take a look at running nodes:

`kubectl get nodes`{{execute}}