FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

VOLUME [ "/app/feedback" ] 
# Anonymous volumes

CMD [ "node", "server.js" ]

# docker run -d -p 3000:80 --rm --name feedback-app $image