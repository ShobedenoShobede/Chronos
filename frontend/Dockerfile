# Use an official Node.js runtime as the base image
FROM node:18

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend app
COPY . .

# Expose the backend port
EXPOSE 5000

# Command to start the backend
CMD ["node", "server.js"]