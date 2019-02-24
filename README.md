#BUILD IMAGE

#docker build <Dockerfile> .

#START DOCKER:
$ docker run --name <name> -d <image> tail -f /dev/null

#STOP DOCKER:
$ docker stop <docker_id>

#USING COMPOSE:
#START:
$ docker-compose up -d

#STOP
$ docker-compose down
============================
#Check

docker ps

===========================
#CONFIG ANSIBLE (control host):

touch /etc/ansible/ansible.cfg

============================
NETWORK:

#Install SSH server for each host:

apt-get update; apt-get install -y openssh-server;service ssh start

#Generate SSH key for each host:

ssh-keygen -t rsa

#Copy public key into authorized_Key file for all hosts:






