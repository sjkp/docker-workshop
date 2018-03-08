# Orcale Database in a Container

What if you have to work against a piece of software that doesn't run on windows, or you are not interested in installing

Docker to the rescue - at least sometimes

I had to do a Azure Data Factory integration with Oracle to test it I installed Oracle in a container and exposed the database to the host

`
docker run -d -p 49160:22 -p 49161:1521 -e ORACLE_ALLOW_REMOTE=true -e ORACLE_ENABLE_XDB=true  wnameless/oracle-xe-11g
`

Browse it at http://localhost:8080/apex/

More https://hub.docker.com/r/wnameless/oracle-xe-11g/