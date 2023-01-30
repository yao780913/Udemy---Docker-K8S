FROM node

WORKDIR /app
# WORKDIR {/the/workdir/path}

COPY package.json /app

RUN npm install
# by default, that working dictionary is the root folder 
# so we need to set WORKDIR /app

COPY . /app
# copy {source}, {dest}
# . means same folder that contains the Dockerfile

EXPOSE 80

CMD ["node", "server.js"]
# RUN vs CMD 
# RUN: when image is created 
# CMD: when container is started