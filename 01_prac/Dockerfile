FROM ubuntu

RUN apt-get update
RUN apt install -y curl
RUN curl -fsSL https://deb.nodesource.com/setup_18.x -o tmp/nodesource_setup.sh
RUN bash tmp/nodesource_setup.sh
RUN apt install -y nodejs 
COPY app.js /home/app/app.js
COPY package.json /home/app/package.json
WORKDIR /home/app

RUN npm install
EXPOSE 3000


