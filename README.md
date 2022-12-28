# Felcloud 
## Les tâches demandées


- La première tâche consiste à créer un rôle Ansible pour configurer un serveur nginx.
- La deuxième tâche consiste à créer un Dockerfile qui permet de lancer une application flask.


## Tâche 1: création du role ansible

- install.yml est pour installer le serveur Nginx.
- service.yml c'est pour gérer le status de Nginx daemon.
- main.yml c'est pour inclure les fichiers install.yml, service.yml et configure.yml
- default.conf c'est pour gérer les configurations par defaut. Il contient les paramètres comme le port, le nom de serveur et les configurations web root.
- handlers/main.yml c'est pour restarter le serveur Ngnix en ajoutant notify task.

## Tâche 2: création du Dockerfile

- Le fichier requirement.txt contient la liste des paquets et des dépendences.
 
#### Création de l’application Flask

- view.py contient l’extrait de code Python
- index.html fournit le contenu de la page à accéder
#### Configuration du fichier Docker
le Dockerfile permet de:
- pull l'image python
- installer les dépendances et les packages dans le fichier requirements.txt
- configurer le container pou le run
#### Construire l’image Docker

```sh
docker run -p 5066:5066 -d flask_docker
```

**BEN DAOUD Maha**
