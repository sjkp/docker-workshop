# Working with container registery


First we need to tag the image 

`
docker tag mynginxstatic sjkpdk.azurecr.io/mynginxstatic
`

Lets see we have a image with a tag now
`
docker images
`

Now lets push it to the remote

`
docker push sjkpdk.azurecr.io/mynginxstatic
`
