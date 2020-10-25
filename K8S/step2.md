# Deploy the API

Startup the API with a single replica:

`kubectl run colisnc --image=rastadidi/colisnc-api:latest --replicas=1`{{execute}}

Then take a look at the newly deployed application (wait until it's ready)

`kubectl get deployments`{{execute}}


Then describe it:

`kubectl describe deployment colisnc`{{execute}}