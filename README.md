## Installation avec docker

- docker-compose build --no-cache
- docker-compose up -d 

Pour Windows : 
```
$ cd docker/nginx/
$ find . -name "*.sh" | xargs dos2unix
```

## Debug docker 

- docker-compose ps
- docker-compose logs -f [CONTAINER(php|node|nginx|db)]

## Mettre à jour bdd

- docker-compose exec php bin/console d:s:u --dump-sql