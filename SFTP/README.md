The easiest way to create a small SFTP server to access your shares.

```
docker container create name=SFTP1 hostname=sftp1.local autostart=yes image=zwck/SFTP expose_ports=yes port:22/TCP=2222  volume:/home/Username/share/=/host/volume01/data command=Username:Password:1337
```
