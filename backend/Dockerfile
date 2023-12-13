FROM node:20-alpine

WORKDIR /src

COPY package*.json ./

RUN npm install

COPY . .
#Port
EXPOSE 3005

RUN npm run build

CMD [ "npm", "run", "start:dev" ]