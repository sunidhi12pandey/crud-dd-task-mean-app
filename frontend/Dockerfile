# ---------- Build Stage ----------
<<<<<<< HEAD
FROM node:22-alpine AS build
=======
FROM node:20-alpine AS build
>>>>>>> sunidhi

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# Production build (uses defaultConfiguration: production)
RUN npm run build

# ---------- Production Stage ----------
FROM nginx:alpine

# Remove default nginx files
RUN rm -rf /usr/share/nginx/html/*

# COPY correct Angular build folder
COPY --from=build /app/dist/angular-15-crud/ /usr/share/nginx/html/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
