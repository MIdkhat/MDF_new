FROM node:8.6-slim

# Set the working directory
WORKDIR /usr/src/app/client

# Copy client package.json
COPY package.json ./

# Install client dependencies
RUN npm install

# Copy client files
COPY ./public ./public
COPY ./src ./src

# Build client
RUN npm run build

# Expose port (if needed)
EXPOSE 3000

CMD ["npm", "start"]
