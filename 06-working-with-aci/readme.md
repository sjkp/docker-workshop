# Working with Azure Container Instances

Get the password
`
az acr credential show --name sjkpdk --query passwords[0].value
`

Create a container instance 

`
az container create --resource-group sjkp.aci --name mynginxstatic --image sjkpdk.azurecr.io/mynginxstatic:latest --cpu 1 --memory 1 --registry-username sjkpdk --registry-password <password> --dns-name-label sjkpaci --ports 80
`

Check that it is online 
`
az container show --resource-group sjkp.aci --name mynginxstatic --query instanceView.state
`
