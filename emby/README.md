Fully working EMBY server.

Here is a working example that assumes presistant config under tank/data/docker-storage
(tank=vdev name)

following folder structure feel free to edit to your needs
```
tank -> multimedia
     -> data/docker-storage/emby
     -> data/docker-storage/dockerSSL-certs
```

CLI copy paste

```
docker container create name=emby hostname=emby.local autostart=yes image=freenas/emby bridged=yes expose_ports=yes port:1900/UDP=1900 port:7359/UDP=7359 port:8096/TCP=8096 port:8920/TCP=8920 volume:/config=/host/tank/data/docker-storage/emby volume:/media=/host/tank/multimedia volume:/sslcerts=/host/tank/data/docker-storage/SSL-certs APP_GID=1337 APP_UID=1337 EDGE=1 UMASK=000 APP_NAME=emby-server
```
