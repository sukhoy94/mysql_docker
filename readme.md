### About
This repository contains simple 
docker-compose.yml file with 2 services:
- db
- phpmyadmin

Also there is a .env file - please do not commit such files
to your repositories, this file here is just a demonstration.

### docker commands

- run all services
```
docker compose up -d
```
after that, you will have mysql instance on http://0.0.0.0:3306 and
phpmyadmin instance on http://0.0.0.0:8080.

You can login with the credentials from your .env

- stop all containers in the system:
```
docker stop $(docker ps -aq)
```

- remove containers db and phpmyadmin with volumes:
```
docker compose down -v
```