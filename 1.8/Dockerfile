FROM ubuntu:16.04 
RUN apt-get update && apt-get -y install curl && curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN mkdir /srv/calculator
WORKDIR /srv/calculator
COPY /calculator /srv/calculator
RUN npm i
EXPOSE 3000
CMD ["npm", "start"]