***
**1.** Read about Docker
***
**2.** Check Docker install by command `sudo docker -v sudo docker -h sudo docker run docker/whalesay cowsay Docker is fun` and redirect to my_work.log
***
**3.** Read Docker documentation
***
**4.** Create image w/ Django site which site create in previous lab by this commands: `docker pull python:3.8-slim` `docker images` `docker inspect python:3.8-slim`
***
**5.** [Link repo Docker](https://hub.docker.com/repository/docker/alexsprynskyi/la-bs)
***
**6.** `sudo docker build -t alexsprynskyi:django .` `sudo docker push alexsprynskyi/la-bs:django`
***
**7.** Run docker image `sudo docker run -it --net=host --rm -p 8000:8000 alexsprynskyi/la-bs:django`
***
**8.** Build Dockerfile.site image `sudo docker build -f Dockerfile.site -t alexsprynskyi/la-bs:monitoring .` and push it to Docker `sudo docker push alexsprynskyi/la-bs:monitoring`
***
**Run both containers** `sudo docker run -it --net=host --rm -p 8000:8000 alexsprynskyi/la-bs:django` `sudo docker run -it --net=host -v $(pwd)/logs:/app/logs alexsprynskyi/la-bs:monitoring`
*** 
**Update READMEFILE and create pull request**
