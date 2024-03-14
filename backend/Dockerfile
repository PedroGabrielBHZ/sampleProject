# Use a lightweight Node.js base image
FROM node:18-alpine

# Create a working directory
WORKDIR /app

# Copy package.json and package-lock.json (if present)
COPY package*.json ./

# Install project dependencies
RUN npm install

# Copy the rest of your project files
COPY . .

# Expose the port your application listens on
EXPOSE 7777

# Command to run when the container starts
CMD [ "node", "app.js" ]
