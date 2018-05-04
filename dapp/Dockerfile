
FROM node:8

EXPOSE 3000

RUN mkdir -p /usr/src/app
COPY . /usr/src/app
WORKDIR /usr/src/app

RUN npm install -g yarn truffle@beta

RUN chmod a+x /usr/local/lib/node_modules/yarn/bin/yarn.js

RUN yarn install 

CMD yarn reset && yarn start

