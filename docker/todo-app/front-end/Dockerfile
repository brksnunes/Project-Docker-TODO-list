FROM node:14-alpine

ENV REACT_APP_API_HOST="todobackend"

ENV REACT_APP_API_PORT=3001

WORKDIR /todo-app/front-end

ADD node_modules.tar.gz .

COPY package.json .

COPY package-lock.json .

RUN npm install

COPY . .

CMD ["npm", "start"]

EXPOSE 3000