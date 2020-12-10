# Call the API

Finally call it:

`http $(minikube ip):$NODE_PORT/colis/CA107308006SI/latest`{{execute}}

Then call it nicely:

`sudo apt-get -y install httpie jq boxes toilet`{{execute}}

```
cat << EOF > colis.sh
#!/bin/bash          
curl -sS http://$(minikube ip):$NODE_PORT/colis/\$1/latest | jq -r '.status' | boxes -d boy | toilet --gay -f term
EOF
chmod u+x colis.sh
```{{execute}}


Finally, cherry on the cake:

`./colis.sh 8Z00136833343`{{execute}}


