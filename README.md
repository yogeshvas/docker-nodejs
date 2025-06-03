Docker COmmands


docker pull ubuntu
docker run ubuntu
docker ps -> gives me all the running containers
docker ps -a -> shows all the images that have run in past
dokcer run -it ubuntu
apt update
apt install vim



docker pull alpine
docker run -it alpine
apk update
apk add vim


PORT MAPPING
docker run -it -p 7990:80 ngnix   (externalPort:InternalPost)


docker logs CONTAINER_ID
docker exec -it CONTAINER_ID bash


Creating your own docker file
1. Create a filename name Dockerfile
2. Basic Commands are as follows
FROM python
ADD app.py /tree/app.py
CMD ["python", "/tree/app.py"]
3. docker build -t python-hello-world .


Removing docker Imgaes
docker image prune