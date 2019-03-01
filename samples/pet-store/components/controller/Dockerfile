# Dockerfile for pet-store controller

FROM node:11.2.0-slim
LABEL maintainer="dev@cellery.io"

RUN mkdir -p /app/controller
WORKDIR /app/controller
COPY package*.json ./
COPY controller.js .

RUN npm install
CMD node controller.js
EXPOSE 80
