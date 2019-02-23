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
