# Images

## Créer une image Docker

```   
docker build -t name .
``` 

* L'argument -t permet de donner un nom à votre image Docker. Cela permet de retrouver plus facilement votre image par la suite.

* Le . est le répertoire où se trouve le Dockerfile. Dans notre cas, à la racine de notre projet.

## Voir les images Docker

``` 
docker images
``` 

## Supprimer les images Docker
``` 
docker rmi 
``` 


# Conteneurs

## Lister les conteneurs 

``` 
docker ps -a
``` 

* L'argument -a permet d'afficher tous les conteneurs (meme les conteneurs qui ne sont pas en cours d'exection)

## Supprimer les conteneurs

Vous pouvez simplement indiquer les identifiants ou les noms des conteneurs séparés par des espaces après la commande docker rm :

``` 
docker rm [CONTAINER ID] [CONTAINER ID]
``` 

## Lancer un  conteneur

``` 
docker run name
``` 

Pour que le conteneur reste actif, il est possible de la lancer des cette facon

``` 
docker run name tail -f /dev/null
``` 


## Entrer dans un conteneurs actif

``` 
docker exec -it [CONTAINER ID] bash
``` 

## Stopper un conteneur

``` 
docker stop [CONTAINER ID]
``` 