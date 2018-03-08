FROM node:8.1.0 as build
ENV NODE_ENV=production
ADD src/gatsby-starter-simple-landing /usr/src/app
RUN npm install --global gatsby-cli
WORKDIR /usr/src/app
RUN npm install
RUN npm run build 
