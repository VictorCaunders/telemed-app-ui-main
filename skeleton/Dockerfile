# Use the official Node.js image as a base
FROM node:22.10.0

# Set the working directory in the container
WORKDIR /telemed-app-ui-main

# Copy package.json and yarn.lock (if available) to the working directory
COPY package.json ./

# Install dependencies
RUN yarn install 

# Copy the rest of your application code to the container
COPY . .

# Build the application
RUN yarn build

# Expose the port that your app runs on
EXPOSE 10000

# Command to run your application (for debugging, change to a shell)
CMD ["/bin/sh"]
