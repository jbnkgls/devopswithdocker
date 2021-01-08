FROM node:latest 

WORKDIR /mydir
COPY . .
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt update
RUN apt install -y nodejs
RUN apt install -y npm
RUN npm install
EXPOSE 8000
CMD FRONT_URL=http://localhost:5000 npm start
