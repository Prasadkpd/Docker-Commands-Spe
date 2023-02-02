# Docker-Commands-Spe

### Run Mongo In Docker Container

1. `docker pull mongo`

1. `docker create mongo`

1. `docker ps –a`

1. `docker run --name mongo_v1 -d -p 27017:27017 mongo`

    Connection Link  -  mongodb://localhost:27017

##### Connect With Bash
   `docker exec -it mongo bash`
