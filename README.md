# Project Description
- The goal of this project was to understand how to deploy python project using docker and build a ci/cd pipeline with github and dockerhub.
- The python application uses flask for routing and server connection. MySQL database.
# Docker
- For python image, the Dockerfile uses node base image. 
- Using the docker-composer file, the configuration settings are defined containing the ports, volume and image information. 
# Github Actions
- Using the github actions ci pipeline workflow configuring is done. 
## Github Action WorkFlow
- Continious integration to github repository.
    - When the code is commited and pushed through the master branch, github action githubrepository.yml (CI to GHCR) runs. The packge python_docker on github also updates.  
- Continious integration to docker hub. 
    - When code is commited with tag V.*.*.*, github action main.yml (CI to docker hub) runs and updates the image on the dockerhub. 
# Running the application locally.
- Pulling the python_docker package you can easily start the server that runs on port 8000. 
- GET "localhost:8000/, returns 'Hello, Docker!'
