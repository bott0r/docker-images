The easiest way to create a small SFTP server to access your shares is via CLI

```
docker container create name=sftp hostname=sftp.local autostart=yes image=freenas/sftp expose_ports=yes port:22/TCP=2222  volume:/home/Username/share/=/host/volume01/data command=Username:Password:1337
```

When using the GUI:

Create a volume  ```/host/share:/home/Username/share```  where Username is the Username of your FTP client
Add the comment  ```Username:Password:1337``` and start
