FROM node:12.16.1

WORKDIR /usr/demo/front-end

COPY ./package*.json /usr/demo/front-end/

RUN npm ci

COPY . /usr/demo/front-end/

RUN npm run lint && npm run build

EXPOSE 3003

CMD [ "npm", "run", "serve" ]