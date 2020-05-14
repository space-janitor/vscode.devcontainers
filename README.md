# vscode.devcontainers

Visual Studio Code development containers

## Docker image creation

``` bash
docker build -t docker.pkg.github.com/space-janitor/vscode.devcontainers/development:skunkworks .
```

## publish

``` bash
docker push docker.pkg.github.com/space-janitor/vscode.devcontainers/development:skunkworks
```

## Startup as a standalone dev container

``` bash
docker-compose up -d
```

## Startup as a vscode remote container

Goto online [documentation](https://code.visualstudio.com/docs/remote/containers) for more information.
