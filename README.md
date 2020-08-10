# vscode.devcontainers

Visual Studio Code development containers

## Prerequisites

| Software   | Notes |
|------------|-------|
| Chocolatey |       |
## Docker image creation

``` bash
docker build -t {image name}:dev .
```

## Start dev container

Modify `container_name` and `image` properties in [docker-compose.yml](./docker-compose.yml) file before using it.

``` bash
docker-compose up -d
```