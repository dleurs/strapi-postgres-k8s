FROM node:13-alpine

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY package.json .
RUN npm install

COPY . .

EXPOSE 1337
CMD ["npm","run","develop"]
