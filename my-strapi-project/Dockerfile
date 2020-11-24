# docker build -t dleurs/strapi-postgres-ovh:0.1.1 .
# docker run --env-file=.env --publish 80:1337 --detach dleurs/strapi-postgres-ovh:0.1.1

FROM node:13-alpine

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app


ENV HOST=""
ENV PORT=""
ENV DATABASE_HOST=""
ENV DATABASE_PORT=""
ENV DATABASE_NAME=""
ENV DATABASE_USERNAME=""
ENV DATABASE_PASSWORD=""
ENV DATABASE_SSL=""
ENV ADMIN_JWT_SECRET=""

COPY package.json .
RUN npm install

COPY . .

EXPOSE 1337
CMD ["npm","run","develop"]
