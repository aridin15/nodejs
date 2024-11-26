# Use the Node.js base image
FROM node:18

# Set the working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy the source code
COPY . .

# Build TypeScript code
RUN npm run build

# Expose the application port
EXPOSE 3000

# Start the app
CMD ["npm", "start"]

