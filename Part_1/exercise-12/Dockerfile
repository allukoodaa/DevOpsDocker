FROM node:16-alpine

EXPOSE 5000

WORKDIR /usr/src/app

# Copy package files and install dependencies
COPY package* .
RUN npm install

# Copy source code
COPY . .

# Build static files
RUN npm run build
# Install package needed to serve static files
RUN npm install -g serve

CMD [ "serve", "-s", "-l", "5000", "build" ]