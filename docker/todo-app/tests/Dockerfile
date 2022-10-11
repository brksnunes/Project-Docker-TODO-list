
FROM mjgargani/puppeteer:trybe1.0

ENV FRONT_HOST="todofrontend"

ENV FRONT_PORT=3000

WORKDIR /todo-app/tests

ADD node_modules.tar.gz .

COPY package.json .

COPY package-lock.json .

RUN npm install

COPY . .

CMD ["npm", "test"]