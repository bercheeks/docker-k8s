# base image
FROM node:14-alpine

# change to the directory 
WORKDIR /usr/app

# install dependencies
COPY ./ ./
RUN npm install

# Default command
CMD [ "npm", "start" ]