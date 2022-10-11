FROM node:14-alpine

WORKDIR /todo-app/back-end

ADD node_modules.tar.gz .

COPY package.json .

COPY package-lock.json .

RUN npm install

COPY . .

CMD ["npm", "start"]

EXPOSE 3001