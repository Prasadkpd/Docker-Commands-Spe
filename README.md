# Docker-Commands-Spe

## Run Mongo In Docker Container

1. `docker pull mongo`

1. `docker create mongo`

1. `docker ps –a`

1. `docker run --name mongo_v1 -d -p 27017:27017 mongo`

    Connection Link  -  mongodb://localhost:27017

   ##### Connect With Bash
   `docker exec -it mongo bash`


## Run Postgress in Docker Container

1. `docker pull postgres`

1. `docker create -v /var/lib/postgres --name postgresdata postgres`

1. `docker run --name con-postgres -p 5432:5432 -e POSTGRES_PASSWORD=admin --mount type=bind,source="$(pwd)"/postgres_data,target=/var/lib/postgres  -d postgres`

1. `docker ps`

1. `docker stop con-postgres`
