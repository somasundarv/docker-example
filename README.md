# docker-example
------------------------------------------

Install Docker : https://docs.docker.com/install/


------------------------------------------

What is Docker  ?  VM vs Docker 

- A server with a long-running daemon process dockerd.
- APIs which specify interfaces that programs can use to talk to and instruct the Docker daemon.
- A command line interface (CLI) client docker.

------------------------------------------

https://docs.docker.com/engine/docker-overview/

Images
Containers

------------------------------------------

getting started : https://docs.docker.com/get-started/

docker run hello-world

------------------------------------------
Example :

https://docs.docker.com/get-started/part2/

git clone https://github.com/dockersamples/node-bulletin-board

cd node-bulletin-board/bulletin-board-app

docker build --tag bulletinboard:1.0 .

docker images

docker run --publish 8000:8080 --detach --name bb bulletinboard:1.0

docker container ls
641d2cafa416        bulletinboard:1.0   "docker-entrypoint.s…"   11 seconds ago      Up 10 seconds       0.0.0.0:8000->8080/tcp   bb
docker rm --force bb
------------------------------------------


Example 

Docker File

docker run -v TMP:/workspace/TMP -it test /bin/bash

docker run   test python3 test.py




