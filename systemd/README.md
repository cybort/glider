## Service

binary file:
```bash
cp glider /usr/bin/
```

service file:
```bash
# copy service file to systemd
cp systemd/glider@.service /etc/systemd/system/
```

config file: ***server***.conf
```bash
# copy config file to /etc/glider/
mkdir /etc/glider/
cp ./config/glider.conf.example /etc/glider/server.conf
```

enable and start service: glider@***server***
```bash
# enable and start service
systemctl enable glider@server
systemctl start glider@server
```
See [glider@.service](glider%40.service)
