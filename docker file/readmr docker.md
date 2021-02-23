
### docker rm $(docker ps -aq)

​
## docker rmi $(docker images -aq)

## docker stop $(docker ps -aq)

### docker rmi $(docker images -aq)

## docker images
## docker run centos
## docker pull ubuntu:18.04d
## docker ps
## docker ps -a
## docker run -d nginx
## docker run docker/whalesay cowsay boo  #create whale
apt update
apt-get install python ansible vim iputils-ping openssh-client -y

docker rmi ubuntu 
docker exec -it ansible_master bash

https://katacoda.com/courses/docker/deploying-first-container

https://docs.docker.com/engine/reference/commandline/commit/


Install the latest LTS version: brew install jenkins-lts
jenkins-lts@YOUR_VERSION
Start the Jenkins service: brew services start jenkins-lts
Restart the Jenkins service: brew services restart jenkins-lts
Update the Jenkins version: brew upgrade jenkins-lts