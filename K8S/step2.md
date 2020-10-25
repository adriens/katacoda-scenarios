# Deploy the API

```
kubectl run colisnc --image=rastadidi/colisnc-api:latest --replicas=1
```


```
kubectl get deployments
```


```
kubectl describe deployment colisnc
```