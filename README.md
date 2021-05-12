# Prove Of Concept Microservices in Spring Boot

## SETUP
### Run Db mysql or anything that you want
docker run -it -d --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=password --restart always -v mysql_data_container:/var/lib/mysql mysql:latest

### Run KeyCloak container
docker run -d --name keycloak -v $(pwd):/tmp -p 8180:8080 -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin quay.io/keycloak/keycloak:13.0.0
