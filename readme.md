## Команды для работы с GIT

```shell
# git submodules clone
git submodule update --init --recursive
```

```shell
# git submodules update
git submodule update --recursive --remote
```

## Команды для запуска Docker Compose
```shell
# custom network creation
# you should write subnet for your custom network
docker network create --subnet=10.5.0.0/16 dev-network
```
