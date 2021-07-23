# Specify base image
# alpine = as small and as compact as possible. Regular node package might contain extra packages like git.
FROM node:alpine

WORKDIR /usr/app

# Copy just package.json
COPY ./package.json ./
# Then install dependencies
RUN npm install
# Then copy rest of files.
COPY ./ ./

# Default command
CMD ["npm", "start"]