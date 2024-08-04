# Use the official Node.js image as a base image
FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy the package.json and package-lock.json files
COPY node-ex-website/package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application code
COPY node-ex-website/ .

# Expose the port the app runs on
EXPOSE 3000

# Define the command to run the application
CMD ["node", "server.js"]
