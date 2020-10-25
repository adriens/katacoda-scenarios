# Make API usable 

Expose the application:

`kubectl expose deployment/colisnc --type="NodePort" --port 8080`{{execute}}


`kubectl describe services/colisnc`{{execute}}

`kubectl get services`{{execute}}