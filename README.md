# hidori/mydns-ipaddress-updater

Notify the IP address to MyDNS.jp

## BUILD

```bash
docker build -f ./Dockerfile -t hidori/mydns-ipaddress-updater .
```

## RUN

```bash
docker run -d \
  --restart=always \
  --name mydns-ipaddress-updater \
  -e ID=<YourID> \
  -e PW=<YourPW> \
  -e INTERVAL=10m \
  hidori/mydns-ipaddress-updater
```
