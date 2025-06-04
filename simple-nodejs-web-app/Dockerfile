# Use official Node.js 18 LTS slim image
FROM node:18-alpine

# Create and set working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to install dependencies
COPY package*.json ./

# Install only production dependencies
RUN npm install

# Copy the rest of your app source code
COPY . .

# Expose the port your Node.js app listens on (usually 3000)
EXPOSE 3000

# Command to run your app (replace app.js if your entry point is different)
CMD ["node", "src/app.js"]