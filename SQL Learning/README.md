# Getting Start
To Getting start with this learning path, you could use the fallowing tools:

- [Docker](https://www.docker.com/)
- [MS SQL Server](https://hub.docker.com/_/microsoft-mssql-server)
- [Azure Data Studio](https://docs.microsoft.com/en-us/sql/azure-data-studio/download?view=sql-server-ver15)
- [VS Code](https://code.visualstudio.com/)

Or whatever relational database you prefer like.
 - [PostgreSQL](https://www.postgresql.org/)
 - [MySQL](https://www.mysql.com/)
 - [SQLite](https://www.sqlite.org/index.html)

Also to practice I recommend use an data warehouse like:
- [AdventureWorks](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms)
- [Northwind](https://github.com/anasmorahhib/Northwind-datawarehouse/blob/master/northwind.sql)
- [WideWorldImporters](https://learn.microsoft.com/en-us/sql/samples/wide-world-importers-install-configure?view=sql-server-ver16&tabs=ssms)
## Docker command to run MS SQL Server:

``` bash
docker run --platform linux/amd64 \
   -e "ACCEPT_EULA=Y"\
   -e "MSSQL_SA_PASSWORD=<Your Strong password>" \
   -p 1433:1433 --name mssql --hostname mssql \
   -d \
   mcr.microsoft.com/mssql/server:2022-latest
``` 

The platform flag is used to specify the platform to run the container on. This is necessary when running on Mac.

## Docker command to run PostgreSQL:

``` bash
docker run \
   -e POSTGRES_USER=postgres \
   -e POSTGRES_PASSWORD=<Your Strong password> \
   -p 5432:5432 --name pgsql --hostname pgsql \
   -d \
   postgres:alpine
```

## Docker command to run MySQL:

``` bash
docker run \
   -e MYSQL_ROOT_PASSWORD=<Your Strong password> \
   -p 3306:3306 --name mysql --hostname mysql \
   -d \
   mysql:latest
```

## Docker command to run SQLite:

``` bash
docker run \
   -p 1433:1433 --name sqlite --hostname sqlite \
   -d \
   sqlite:latest
```

## Table of Contents

### [[Insert Statement]]
### [[Select Statement]]
### [[Update Statement]]
### [[Delete Statement]]
### [[Columns]]
