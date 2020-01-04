FROM ubuntu 

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs git

RUN git clone https://github.com/docker-hy/backend-example-docker.git

EXPOSE 8000
WORKDIR /backend-example-docker
RUN npm install
CMD npm start 