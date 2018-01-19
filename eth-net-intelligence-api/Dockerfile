FROM node:8-alpine

RUN apk add --update git

RUN git clone https://github.com/cubedro/eth-net-intelligence-api.git

WORKDIR /eth-net-intelligence-api

RUN npm install

CMD ["node", "app.js"]
