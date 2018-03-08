# .NET Core in Containers
Lets build a .NET core application in a linux container


Worthy mentions multi-stage build

.dockerignore 

`
docker build . -t mydotnet
`

`
docker run -p 8082:80 mydotnet
`