# SharePoint Framework in a Docker Container

Why ?? 

It is just an example of how many tools are actually available in containers, so you don't have to pollute you machine installing them. 

`
docker run -it --rm --name spfx-helloworld -v ${PWD}:/usr/app/spfx -p 5432:5432 -p 4321:4321 -p 35729:35729 waldekm/spfx
`