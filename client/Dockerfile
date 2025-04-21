# Use official Node image
FROM node:20

# Set working directory inside container
WORKDIR /client

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all other source files
COPY . .

# Expose the Vite default port
EXPOSE 5173

# Run vite dev server
CMD ["npm", "run", "dev"]