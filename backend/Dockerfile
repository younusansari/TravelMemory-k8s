# Use official Node.js image
FROM node:18-alpine

# Create app directory
WORKDIR /app

# Copy package files first (for better caching)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the application
COPY . .

# Expose the app port (use your PORT env, e.g., 3001)
EXPOSE 3001

# Start the application
CMD ["node", "index.js"]