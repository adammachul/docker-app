# Create image based on the official Node 6 image from dockerhub
FROM node:6

# Install vim
RUN apt-get update && apt-get install -y vim

# Create a directory where our app will be placed
RUN mkdir -p /usr/angular-client

# Change directory so that our commands run inside this new directory
WORKDIR /usr/angular-client

# Get all the code needed to run the app
COPY . /usr/angular-client

# Install dependecies
RUN npm install

# Expose the port the app runs in
EXPOSE 4200

# Serve the app
CMD ["npm", "start"]


