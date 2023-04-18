FROM ubuntu:20.04
WORKDIR /root/.ssh/
RUN apt-get update && apt-get install nginx -y && apt-get install openssh-server -y
COPY . .
CMD service nginx start && service ssh start && sleep infinity

