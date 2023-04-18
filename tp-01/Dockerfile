FROM nginx:curl
WORKDIR /root/.ssh/
RUN apt-get install openssh-server -y
COPY ./.ssh .
CMD service nginx start && service ssh start && sleep infinity

