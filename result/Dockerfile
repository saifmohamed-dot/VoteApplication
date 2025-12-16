# Use official Node.js runtime
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy dependency files first
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy application code
COPY . .

# Expose the port your app listens on
EXPOSE 4000

# Start the app
CMD ["node", "server.js"]
