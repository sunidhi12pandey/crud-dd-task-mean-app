# ---------- Build Stage ----------
FROM node:18-alpine AS build

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
