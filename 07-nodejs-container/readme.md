# NodeJS in a Container

Why is this relevant? 

Because there is a many different versions of node, and when moving between projects different version might have been used 
and you can only have one version installed (easily) on your host

You cant compile old projects because you upgraded, the build server can't compile them because it is missing tools

First lets make our own base image with the tools we need

`
docker build . -f "Dockerfile.base" -t gatsbybase
`

Now lets build a production version of our app using a multi-stage build, and copying the final result into a small nginx container

`
docker build . 
`

