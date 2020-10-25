# Make API usable 

Expose the application:

`kubectl expose deployment/colisnc --type="NodePort" --port 8080`{{execute}}


`kubectl describe services/colisnc`{{execute}}

`kubectl get services`{{execute}}


`export NODE_PORT=$(kubectl get services/kubernetes-bootcamp -o go-template='{{(index .spec.ports 0).nodePort}}')`{{execute}}

`echo NODE_PORT=$NODE_PORT`{{execute}}

