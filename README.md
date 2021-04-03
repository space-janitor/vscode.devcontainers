# vscode.devcontainers

Visual Studio Code development container.

## Environment file

Use the following template to create environment file

```environment
MYSQL_DATABASE=databasename
MYSQL_ROOT_PASSWORD=password
DEVCONTAINER_HOSTNAME=SpaceJanitor
DEVCONTAINER_HOME=/home/betancourtca
```

## Expected home files & directories

This files will be mapped by docker-compose.yml

### ~/.aws

AWS configuration folder

### ~/.npmrc

Sample template to create .npmrc in your home directory

```npm
strict-ssl=true
//npm.pkg.github.com/:_authToken=token here
init.license=MIT
registry=https://npm.pkg.github.com/space-janitor
```

## Start dev container

```bash
docker-compose up -d
```

## Troubleshooting

You might get a password error due to not accessing database through localhost.

For mysql 8.x run the following cmd as a query (Replace `root` and `password` as required based on the values in your `.env` file).

```bash
alter user root@'%' identified with mysql_native_password by "password";
```
