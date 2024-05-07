# Use the official Node.js image as base
FROM node:latest

# Set working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port your app runs on
EXPOSE 3000

# Command to run your app using npm
CMD ["npm", "run", "start:prod"]
