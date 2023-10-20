# Why for the love of God?

```bash
p=$(tr -dc A-Za-z0-9 </dev/urandom | head -c 18)
echo "MYSQL_ROOT_PASSWORD=$p" > .my.env
chmod 600 .my.env
```

```bash
docker-compose up -d

# Send the sql to mysql somhow...
docker exec mysql mysql < *.sql

# Should I copy it in in the build stage?

```
