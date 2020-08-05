# Udacity_microservices-Udagram
Refactor Udagram App into Microservices and Deploy

# Project Detail:

project has docker-compose file to run docker containers, each services like : frontend service, rest API user service, and rest API feed service ahve their own docker image.  both user and feed uses the same port.
Also, the project has kubernete which run each docker dontainer inside pod in cluster.

# Points covered:
* /feed and /user backends are separated into independent projects.
* Project includes Dockerfiles to successfully create Docker images for /feed, /user backends, project frontend, and reverse proxy.
* Integrated CI/CD pipeline by using Travis CI and docker and Kubernets.
* Impemented Reverse proxy
* Horizontal scaling with kubernet
