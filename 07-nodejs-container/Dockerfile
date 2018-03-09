FROM gatsbybase as build
ENV NODE_ENV=production
ADD src/gatsby-starter-blog /usr/src/app
WORKDIR /usr/src/app
RUN yarn install
RUN npm run build 

FROM nginx:alpine
WORKDIR /usr/share/nginx/html
COPY --from=build /usr/src/app/public .