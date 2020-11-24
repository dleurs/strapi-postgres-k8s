# docker build -t dleurs/strapi-postgres-ovh:0.1.1 .
# docker run --env-file=.env --publish 80:1337 --detach dleurs/strapi-postgres-ovh:0.1.1

FROM node:13-alpine

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY package.json .
RUN npm install

COPY . .

EXPOSE 1337
CMD ["npm","run","develop"]
