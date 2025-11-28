FROM node:20-alpine

# Create app directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install --production

# Copy the rest of the code
COPY . .

# Set environment variables
ENV PORT=3000

# Expose the port the app runs on
EXPOSE 3000

# Start the backend
CMD ["npm", "start"]
