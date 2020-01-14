FROM ubuntu

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs git

RUN git clone https://github.com/docker-hy/frontend-example-docker.git
EXPOSE 5000
ENV API_URL=http://localhost:8000
WORKDIR /frontend-example-docker

RUN npm install

CMD npm start

