#Stage 1:
#Use official Node.js image as the base image
FROM node:18-alpine AS builder
#set working directory
WORKDIR /app
#copy package.json and package-lock.json
COPY package*.json ./
#install dependencies
RUN npm install
#copy all the files
COPY . .
#expose the preferred port
EXPOSE 9000
#run the node.js application
CMD [ "npm", "start" ]
