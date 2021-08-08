# Chercher un ridet

Récupérer les détails de l'entreprise dont le ridet est `0426049` :

```
http :8080/ridet/0426049
```{{execute}}

Tester que chercher une entreprise avec un ridet qui n'existe pas renvoie bien une erreur [404](https://fr.wikipedia.org/wiki/Erreur_HTTP_404) :

```
http :8080/ridet/04260499
```{{execute}}