Cette fois-ci, on cherche, via un mot-clé (`042604`) et on veut récupérer une collection d'entreprises candidates :

```
http :8080/ridets?q=04260
```{{execute}}

Voyons ce qui se passe avec plus de hits :

```
http :8080/ridets?q=sports&page=1
```{{execute}}

... jusqu'à tomber sur une page vide :


```
http :8080/ridets?q=sports&page=100
```{{execute}}