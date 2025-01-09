FROM node:18-alpine AS base

WORKDIR /app

COPY ./package.json yarn.lock* package-lock.json* ./

RUN yarn install

COPY . .

RUN yarn build

EXPOSE 3001

CMD ["yarn", "start"]