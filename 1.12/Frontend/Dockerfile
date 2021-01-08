FROM node:latest 

WORKDIR /mydir
COPY .. ..
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt update
RUN apt install -y nodejs
RUN apt install -y npm
EXPOSE 5000
CMD API_URL=http://localhost:8000 npm start
