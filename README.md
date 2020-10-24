# vscode.devcontainers

Visual Studio Code development containers

## Start dev container

``` bash
docker-compose up -d
```

## MySQL

### Environment file

Use the following template to create environment file

``` environment
MYSQL_DATABASE=databasename
MYSQL_ROOT_PASSWORD=password
```

### local development

For mysql 8.x run the following cmd as a query (Replace `root` and `password` as required based on the values in your `.env` file).

``` bash
alter user root@'%' identified with mysql_native_password by "password";
```
