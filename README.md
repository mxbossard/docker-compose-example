
## Build 1
Création d'un premier projet compose qui démarre simultanément les 2 conteneurs suivant :
* mysql
* wordpress

La configuration est réalisée au format yaml dans le fichier docker-compose.yml.

``` bash
docker-compose config
docker-compose up
```

Pour démarrer en mode démon :
``` bash
docker-compose up -d
```

Pour lister les conteneurs démarrés :
``` bash
docker-compose ps
```

Pour afficher les logs :
``` bash
docker-compose logs
```

Pour redémarrer les conteneurs :
``` bash
docker-compose stop
docker-compose start
```
ou bien :
``` bash
docker-compose restart
```

Pour tuer les conteneurs :
``` bash
docker-compose kill
```
Cela détruit les conteneurs. Tout ce qui était stoqué dedans est perdu.
La base de données mysql est configuré pour utiliser un volume persistant, la base de données sera donc conservée.

Pour lister les volumes existants :
``` bash
docker volume ls
```

