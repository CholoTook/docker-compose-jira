# Why for the love of God?

## Step 1, Set up passwords

```bash
# Generate a random root password
p=$(tr -dc A-Za-z0-9 </dev/urandom | head -c 18)
echo "MYSQL_ROOT_PASSWORD=$p" > .my.env
chmod 600 .my.env

# Replace with your own username and password...
vi docker-entrypoint-initdb.d/setup-jira.sql 
```

## Step 2, Build and deploy

```bash
docker build Jira/
docker-compose up -d
```
