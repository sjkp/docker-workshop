# .NET Core in Containers
Lets build a .NET core application in a Linux container

Microsoft provides some base images that we can use. 

Because we want the image to be as small as possible, we create a multi-stage Dockerfile. 

Multi-stage means that we can have one Dockerfile, but our bulid base image doesn't have to be the same as our runtime image. 

In addition we can simplify the process of copying files into the image, using a `.dockerignore` file. Same concept for `.gitignore` 
content that we wont the docker engine to ignore 

Lets try to build our image

`
docker build . -t mydotnet
`

`
docker run -p 8082:80 mydotnet
`