FROM ansible/ubuntu14.04-ansible:latest
EXPOSE 22
RUN apt-get update && apt-get install -y \
    openssh-server
RUN service ssh start
RUN ssh-keygen -t rsa -q -N "" -f /root/.ssh/id_rsa
CMD touch /etc/ansible/ansible.cfg
CMD tail -f /dev/null
