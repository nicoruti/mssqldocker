# MSSQL 2019 Docker container

Image is hosted on [Dockerhub](https://hub.docker.com/repository/docker/nicoruti/mssql).

## Usage
Use the following command to start:

```
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=<admin-password>' -e 'MSSQL_DB=<db-name>' -e 'MSSQL_USER=<username>' -e 'MSSQL_PASSWORD=<password>' -p 1433:1433 microsoft/mssql-server-linux:2017-latest
```

## Variables
* ACCEPT_EULA: Must be 'Y' if you accept the MSSQL EULA
* SA_PASSWORD: The system admin password
* MSSQL_DB: The database name
* MSSQL_USER: The database user to create
* MSSQL_PASSWORD: The database user password

Note: Microsoft requires strong passwords, otherwise, the server does not start.