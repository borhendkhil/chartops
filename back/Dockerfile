# backend/Dockerfile
FROM node:16

# Set the working directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy the source code
COPY . .

# Build the application
RUN npm run build

# Expose the application's port
EXPOSE 3000

# Start the application
CMD ["node", "dist/main.js"]
