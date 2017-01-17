Prerequisits: Working MongoDB with known username and password. Check MongoDB for Freenas

Typicall setup:

``` ROOT_URL http://IP.IP.IP.IP:3000 ```
``` MONGO_URL mongodb://myuser:password123@IP.IP.IP.IP:27017/rocketchat ```

Start 
 done.
 
 Browse to http://IP.IP.IP.IP:3000
 
 chat


#CLI snippet 
If MongoDB-database with the name *rocketchat* has been created using *myuser* as user and *password123* as password  (freenas.local can/should be replaced with IP)

```
docker container create name=rocketchat hostname=rocketchat.local autostart=yes image=freenas/rocketchat expose_ports=yes volume:/app/uploads=/host/tank/data/docker-storage/rocketchat/ ROOT_URL=http://freenas.local:3000 MONGO_URL=mongodb://myuser:password123@freenas.local:27017/rocketchat
```
