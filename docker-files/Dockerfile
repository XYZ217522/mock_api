FROM node:17-alpine3.14

# Bundle app source
COPY . /app

# Create app directory
#WORKDIR /app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY ./package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Create app directory
WORKDIR /app

# Bundle app source
COPY . /app

#EXPOSE 3000

CMD [ "node", "src/index.js" ]
