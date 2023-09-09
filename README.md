# Codeigniter-docker

basic files to use [docker](https://www.docker.com/) as local environment for development with [Codeigniter](https://www.codeigniter.com/). My 2 cents here.

What we have here:

- A Dockerfile with the settings that codeigniter needs to work fine with [php](https://www.php.net/) environment.

- docker-compose.yml to turn it more easy to handle the container with start and stop cli commands

Just put in your root folder and be happy =D. Remember to erase this _public_ folder here before start to use on your environment

## troubleshooting

Set permission on cache folder to work fine

## docker-compose.yml

I just add some containers to work with localdatabase and phpmyadmin on docker. If you already install docker just do docker compose -f "docker-compose.yml" up -d --build in your terminal and have fun.

That command will create an localdata as docker volume folder on you root folder, put this folder on .gitignore to avoid up that folder to github. That approach is only to local development.

Feel free to rename the containers on docker-compose file