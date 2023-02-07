# Use the official Node.js version 12 Alpine image as the base image
FROM node:12-alpine

# Set the working directory in the container to /app
WORKDIR /app

# Copy the package.json file to the container
COPY package.json .

# Install the dependencies using npm
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose port 80
EXPOSE 80

# Start the application using the appropriate command
CMD ["npm", "start"]
