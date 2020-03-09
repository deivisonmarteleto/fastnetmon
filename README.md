# docker-fastnetmon +  Telegram ( python )

Base [FastNetMon](https://github.com/pavel-odintsov/fastnetmon) 

## Como executar:

Para iniciar o contêiner, execute o comando:

```bash
docker run \
  --name fastnetmon \
  --detach \
  --privileged \
  --net host \
  --volume /etc/localtime:/etc/localtime:ro \
  --volume fastnetmon:/fastnetmon \
  --volume fastnetmon-attacks:/var/log/fastnetmon_attacks \
  dmarteleto/fastnetmon
```

## Como parar / iniciar / reiniciar um contêiner?

Use os comandos para gerenciar o contêiner.

    docker stop fastnetmon
    docker start fastnetmon
    docker restart fastnetmon

## Como iniciar o cliente FastNetMon?

Para iniciar o cliente, use o comando

    docker exec --tty --interactive fastnetmon /opt/fastnetmon/fastnetmon_client





