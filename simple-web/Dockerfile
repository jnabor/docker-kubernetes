# Use an existing docker image as base
FROM node:alpine

WORKDIR /usr/app

# Download and install a dependencies
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Tell the image what to do when it starts the container
CMD ["npm", "start"]

#run command
# docker run -p <host port>:<container port> <image>