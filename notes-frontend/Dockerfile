FROM node:alpine

WORKDIR /app

COPY package*.json ./
RUN npm install


COPY . .

RUN npm build --prod

EXPOSE 80

CMD [ "npx", "serve", "-s", "dist" ]

