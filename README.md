# Why for the love of God?

## Step 0

```bash
vi MySQL/setup-jira.sql ...
docker build MySQL/
```

## Step 1

```bash
p=$(tr -dc A-Za-z0-9 </dev/urandom | head -c 18)
echo "MYSQL_ROOT_PASSWORD=$p" > .my.env
chmod 600 .my.env
```

## Step 2

```bash
docker-compose up -d
```

## Step 3



## Rough notes

docker build Jira/
docker build MySQL/
