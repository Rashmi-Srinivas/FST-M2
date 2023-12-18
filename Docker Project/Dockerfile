# Set base image
FROM node:18-alpine

# Create a working Directory
WORKDIR /usr/app

# Copy package.json from host to wrok directory
COPY ./package.json ./

# Install dependencies for the app
RUN npm install

#Copy everything to container
COPY ./ ./

# Start the redis server
CMD [ "npm", "start" ]