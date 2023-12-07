# Use an official Node.js runtime as a base image
FROM node:latest

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY app_files/package.json ./
COPY app_files/package-lock.json ./

# Install application dependencies
RUN npm install

# Copy the application source code to the container's working directory
COPY app_files/ ./

# Expose port 8080
EXPOSE 8080

# Command to run the application
CMD ["node", "app.js"]  # Replace "app.js" with your main Node.js file