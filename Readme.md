Golang & GraphQL

https://www.howtographql.com/graphql-go/0-introduction/

start mysql server with docker

    docker run -p 3306:3306 --name mysql -e MYSQL_ROOT_PASSWORD=dbpass -e MYSQL_DATABASE=hackernews -d mysql:latest

create a Table names hackernews for our app

    docker exec -it mysql bash
    mysql -u root -p
    CREATE DATABASE hackernews;

run the server

    go run server.go