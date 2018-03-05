# Create a simple static web site using nginx 

Find the base image in docker hub: https://hub.docker.com/_/nginx/ 

Lets run the image by volume mounting our content into the container

`
docker run --name mynginx -v j:/projects/docker-workshop/01-simple-nginx/src:/usr/share/nginx/html:ro -p 5005:80 -d nginx 
`

To remove the running container

`
docker rm -f mynginx
`


# Build an image with our content embedded

`
docker build . -t mynginxstatic
`

view your images

`
docker images
`


To run you container locally

`
docker run -p 5003:80 mynginxstatic
`

Or in detatched mode

`
docker run -d -p 5003:80 mynginxstatic
`

Now you will not see the logs, if you want to view the log output

`
docker logs -f 5d8 
`

Where 5d8 is part of the container id, you can get it with 

`docker ps`