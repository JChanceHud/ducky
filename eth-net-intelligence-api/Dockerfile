FROM node:8-alpine

RUN apk add --update git

RUN git clone https://github.com/cubedro/eth-net-intelligence-api.git

WORKDIR /eth-net-intelligence-api

RUN npm install && \
    npm install -g pm2

COPY app.json .

CMD ["/usr/local/bin/pm2", "start", "--no-daemon", "app.js"]
