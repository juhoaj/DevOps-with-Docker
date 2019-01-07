FROM ubuntu:16.04 
RUN apt-get update && apt-get -y install curl && curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN mkdir /srv/palvelu
WORKDIR /srv/palvelu
COPY /frontend-example-docker /srv/palvelu
RUN npm i
EXPOSE 5000
CMD ["npm", "start"]