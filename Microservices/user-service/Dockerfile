# Use the official Node.js 18 Alpine image as parent image
FROM node:18-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json to install dependencies
COPY package.json ./

# Install packages
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the user-service port
EXPOSE 3000

# Command to run the application
CMD ["node", "app.js"]
