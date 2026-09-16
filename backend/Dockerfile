<<<<<<< HEAD
FROM node:22-alpine
=======
FROM node:20-alpine
>>>>>>> sunidhi

WORKDIR /app

COPY package* ./
RUN npm install

COPY . .

EXPOSE 8080

CMD ["node", "server.js"]
