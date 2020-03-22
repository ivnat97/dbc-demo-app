FROM node:12.16.1-alpine

WORKDIR /usr/demo/back-end

COPY ./package*.json /usr/demo/back-end/

RUN npm ci

COPY . /usr/demo/back-end/

RUN npm run lint

EXPOSE 3002

CMD [ "npm", "run", "start" ]