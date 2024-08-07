# Use an official Node.js runtime as a parent image
FROM node:18-slim

# Step 4.1 - Set the working directory
WORKDIR /usr/src/app

# Step 4.2 - Copy npm dependencies
COPY package*.json ./

# Step 4.3 - Install dependencies
RUN npm install

# Copy app source code
COPY . .

# Update npm packages
RUN npm update

# Set environment variable to address OpenSSL issue
ENV NODE_OPTIONS=--openssl-legacy-provider

# Expose port and start the application
EXPOSE 8080
CMD ["npm", "start"]
