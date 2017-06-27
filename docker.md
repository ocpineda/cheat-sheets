
## TODO
- Check out Docker Compose
  <https://docs.docker.com/compose/overview/>

**run**  
`docker run -d -p 80:80 --name webserver nginx`

**container details**  
`docker ps`

**Stop webserver**  
`docker stop webserver`  

**Start server**  
`docker start webserver`  

**See a stopped container in ps**  
`docker ps -a`

**Remove a container, but not image**  
`docker rm -f webserver`  

**List images**  
`docker images`  

**Remove a Docker image**  
`docker rmi [image name]`


**One liner to stop / remove all of Docker containers:**  
```
docker stop $(docker ps -a -q)   
docker rm $(docker ps -a -q)
```

**SSH to container**  
docker exec -it (mycontainer) bash

**build container with a tag labeled "brs"**  
`docker build -t brs .`

**Run that brs container via Jboss port **  
`docker run -d -p 8080:8080 brs`  
