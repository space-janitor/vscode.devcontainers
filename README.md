# vscode.devcontainers

Visual Studio Code development containers

## Docker image creation

``` bash
docker build -t space-janitor:dev .
```

## Startup as a standalone dev container

``` bash
docker-compose up -d
```

## Startup as a vscode remote container

Goto online [documentation](https://code.visualstudio.com/docs/remote/containers) for more information.

## Notes

### SUDO

- SUDO support added. See [Creating a non-root user](https://code.visualstudio.com/docs/remote/containers-advanced#_creating-a-nonroot-user) for more information.

### AWS

Click [here](https://aws.amazon.com/cli/) for instruction on installing AWS CLI v2.x.

Click [here](https://aws.amazon.com/serverless/sam/) for instructions on installing AWS SAM CLI. Have includeded modified [linuxbrew.sh](./linuxbre.sh) given that this configuration default user is `root`.


