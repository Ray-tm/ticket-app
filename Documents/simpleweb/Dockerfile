#base image
FROM node:14-alpine

#tells where to put the files. if directory doesn't exist, it will be made
#For a node.js app it doesnt matter where you put the files in a linux system
WORKDIR /usr/app

COPY ./package.json ./
RUN npm install
RUN npm install vim
COPY ./ ./

CMD ["npm", "start"]