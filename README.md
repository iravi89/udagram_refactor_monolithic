# Udacity_microservices-Udagram
Refactor Udagram App into Microservices and Deploy

# Project Detail:

project has docker-compose file to run docker containers, each docker container has pne service whcih are : frontend service, rest API user service, and rest API feed service. both user and feed use the same port and reverseproxy control the incoming traffic between them.

Also, the project has kubernete which run each docker dontainer inside pod in cluster.

1- run docker compose docker-compose up

2- port-forward kubectl port-forward service/frontend 8100:8100 kubectl port-forward service/reverseproxy 8080:8080

# Points covered:
* /feed and /user backends are separated into independent projects.
* Project includes Dockerfiles to successfully create Docker images for /feed, /user backends, project frontend, and reverse proxy.
* Integrated CI/CD pipeline by using Travis CI and docker and Kubernets.
* Impemented Reverse proxy
* Horizontal scaling with kubernet
