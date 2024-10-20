# dbi-server

## 1. start up

```bash
docker run \
    -p 9002:80 \
    --name dbi-server \
    -v ./nginx/conf/nginx.conf:/etc/nginx/nginx.conf \
    -v ./nginx/conf/conf.d:/etc/nginx/conf.d \
    -v ./nginx/log:/var/log/nginx \
    -v ./nginx/html:/usr/share/nginx/html \
    -d nginx:latest
```

## 2. mv game to nginx dir

```
mv game nginx/html/Nintendo/Switch
```

## 3. use dbi via home server

- https://github.com/rashevskyv/dbi/blob/main/README_ENG.md#home-server
