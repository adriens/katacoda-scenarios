# Postres install

To make this tutorial playable anywhere (and play with PostgreSQL versions), we'll use
docker.

First, update your system :

`sudo apt-get update`{{execute}}

Then properly install docker:

```
sudo apt-get remove docker docker-engine docker.io
sudo apt install docker.io
sudo systemctl start docker
sudo systemctl enable docker
docker --version
```{{execute}}

Then locally install postgreSQL client :

`sudo apt-get install postgresql-client`{{execute}}

Next, pull and boot PostgreSQL:

```
sudo docker pull postgres:13.1
sudo docker run --rm --name pg-docker -e POSTGRES_PASSWORD=docker -d -p 5432:5432 postgres:13.1
```{{execute}}

Finally connect and create a demo database:

```
export PGPASSWORD=docker
## create a dedicated database for the demo
psql -h localhost -U postgres -d postgres -c "create database demo"
psql -h localhost -U postgres demo
```{{execute}}

We are done, let's put the interesting thing now : deal with the database.