# Make API usable 

Expose the application:

`kubectl expose deployment colisnc --external-ip="172.17.0.34" --port=8080 --target-port=8080`{{execute}}