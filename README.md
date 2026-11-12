# sdm-jdbc

Docker run:
docker run -d --name mariadb_container -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=jdbcex -e MYSQL_USER=myuser -e MYSQL_PASSWORD=pass -p 3306:3306 -v mariadb_data:/var/lib/mysql mariadb:latest

Docker interactive terminal:
docker exec -it mariadb_container mariadb -u root -p

Run the sql scripts from create.sql and insert.sql

If there are issues with the DB driver, Maven - reload all Maven projects