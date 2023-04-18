# Use an official Node.js runtime as a parent image
FROM node:14-alpine

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install any needed dependencies specified in package.json
RUN npm install

# Copy the rest of the application files to the container
COPY . .

# Set the environment variable for the app
ENV NODE_ENV production

# Expose port 3000
EXPOSE 8080

# Start the application
CMD sleep 10 && npm run start
