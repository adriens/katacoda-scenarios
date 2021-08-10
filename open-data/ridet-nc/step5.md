Cette fois-ci, on cherche, via un mot-clé (`042604`) et on veut récupérer une collection d'entreprises candidates :

```
http :8080/ridets q==04260
```{{execute}}

Voyons ce qui se passe avec plus de hits :

```
http :8080/ridets q==sports page==1
```{{execute}}

Formatons en csv pour rendre les choses plus lisibles :

```
http :8080/ridets q==sports page==1 |
jq -r '["rid7","denomination", "libelleCommune","codeApe"], (.[] |
[.rid7,.denomination,.libelleCommune,.codeApe]) |
@csv'
```{{execute}}

Formatons en tableau scrollable :

```
http :8080/ridets q==sports page==1 |
jq -r '["rid7","denomination", "libelleCommune","codeApe"], (.[] |
[.rid7,.denomination,.libelleCommune,.codeApe]) |
@csv' |
column -t -n -s, |
less -S
```{{execute}}


Cherchons la dernière page : il suffit de tomber sur une page vide :


```
http :8080/ridets q==sports page==100
```{{execute}}
