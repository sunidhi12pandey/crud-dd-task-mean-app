FROM node:22-alpine

WORKDIR /app

COPY package* ./
RUN npm install

COPY . .

EXPOSE 8080

CMD ["node", "server.js"]
