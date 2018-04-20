# Developing a PHP and MYSQL application using Docker-Compose

## File Structure

The file structure needs to be as follows:

.
+-- docker-compose.yml
+-- Dockerfile
+-- mysql_init
  +-- dbcreation.sql
+-- webapp
  +-- cloudtech.php

Cloudtech.php is the PHP script that accesses the SQL database and retrieves the value.
Dbcreation.sql is a file that creates a table and enters a value in it. 

## How to run it:

To spin up the containers and obtain a functioning app, please run the below commands:

```bash
docker-compose build
docker-compose up -d
```
## How to test:

To test access the following link:
http://127.0.0.1:80/cloudtech.php

