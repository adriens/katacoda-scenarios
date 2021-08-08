# Installer l'API

Télécharger et exécuter l'[API Ridetnc](https://github.com/adriens/ridetnc-api) :

```
sudo docker run -d --name ridets-nc -p 8080:8080 rastadidi/ridetnc-api:latest
```{{execute}}

Vérifier que l'API tourne :

```
sudo docker ps
```{{execute}}