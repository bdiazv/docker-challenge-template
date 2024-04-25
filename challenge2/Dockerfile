# Use the official Node.js image as base
FROM node:alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy server.js into the container
COPY server.js .

# Expose the port the app runs on
EXPOSE 3000

# Command to run the server
CMD ["node", "server.js"]
