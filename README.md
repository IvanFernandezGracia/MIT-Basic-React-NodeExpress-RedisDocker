# MIT-Basic-React-NodeExpress-RedisDocker


<!-- DESCRIPTION -->
## Description
Basic 3 level application, frontend, backend and database. Frontend is developed with React, Backend with Node Express and database with Redis on Docker. All hosted locally.

<!-- Architecture -->
## Architecture
![Sin título](https://user-images.githubusercontent.com/48660555/155814033-e585d523-8675-4798-8d11-048e2709f0e4.png)

<!-- Frontend - Backend and Database -->
## Frontend & Backend & Database
![Captura de pantalla 2022-02-25 193549](https://user-images.githubusercontent.com/48660555/155814049-cec76e31-d464-48b0-a271-5e628a7f9d3b.png)


<!-- RUN -->
## Step Run 
1. Run react application and use superagent for communication of api Rest in backend (static file into public folder)
2. Run server with nodejs and express, where the api endpoints are created and the connection with the Redis database in docker.
3. Run redis database with docker and its command line container.

## Step Run React App & Server Express
1. Install dependencies `$ npm install`
2. Run React app static files and server express `$ node index.js`

## Step Run Redis and Redis Commander
1. Create/download image redis `$ docker pull redis:latest`
2. Verify image redis `$ docker images`
3. Run container redis`$ docker run --name my-redis -p 6379:6379 -d redis`
4. Verify container redis run `$ docker ps -a`
5. Create/download image redis commander`$ docker pull rediscommander/redis-commander:latest`
6. Verify image redis commander `$ docker images`
7. Get IPAddress redis server host`$ docker inspect my-redis -f "{{json .NetworkSettings.Networks}}"`
8. Run container redis commander`$ docker run --name my-redis-commander -p 8081:8081 --env REDIS_HOSTS=local:172.17.0.2`
9. Verify container run`$ docker ps -a`

<!-- ROADMAP -->


<!-- LICENSE -->
## Licence 
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) *The MIT License*

<!-- CONTACT -->
## Contact
Ivan Alejandro Fernandez Gracia  
:email: ivan.fernandez.g@usach.cl  
:telephone_receiver: +56-961214718  
Fullstack & Mobile Developer  
Mechanical Engineering  
Universidad de Santiago de Chile
