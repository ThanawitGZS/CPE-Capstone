# Stage 1: build frontend
# FROM node:18 as frontend-build
# WORKDIR /app
# COPY Frontend/package*.json ./
# RUN npm install
# COPY Frontend/ ./
# RUN npm run build

# Stage 2: build nginx image
FROM nginx:alpine
COPY nginx.conf /etc/nginx/nginx.conf
COPY ./dist /usr/share/nginx/html
# COPY --from=frontend-build /app/dist /usr/share/nginx/html