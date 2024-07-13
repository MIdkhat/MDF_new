FROM node:8.6-slim

# Set the working directory
WORKDIR /usr/src/app/server

# Copy server package.json
COPY package.json ./

# Install server dependencies
RUN npm install

# Copy server files
COPY ./bin ./bin
COPY ./routes ./routes
COPY ./app.js ./app.js

# Expose port (if needed)
EXPOSE 3001

CMD ["npm", "run", "start"]
