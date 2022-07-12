# Postgres 13 DB
This DB has the objective of the store all the information of the analysis inside a local database. This db is running inside Docker and uses a folder to have data persistence.

## Instruction
To run the local db first, you need to create a local folder
```
mkdir data_postgres
```
Then you need to run Docker compose
```
docker-compose up
```
To connect to this database, you will use the following credentials:

```
User: root
Password: root
Ports: 5232
```