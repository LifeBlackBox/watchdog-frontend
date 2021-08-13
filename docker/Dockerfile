FROM node:lts-alpine

RUN npm install -g http-server

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

COPY ./docker/entrypoint.sh ./entrypoint.sh

ENTRYPOINT ["sh", "entrypoint.sh"]
