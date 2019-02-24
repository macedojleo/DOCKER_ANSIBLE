FROM mysql:latest
EXPOSE 22
RUN apt-get update && apt-get install -y \
    openssh-server
RUN service ssh start
#CMD rm -f /root/.ssh/id_rsa*
RUN ssh-keygen -t rsa -q -N "" -f /root/.ssh/id_rsa
CMD tail -f /dev/null
