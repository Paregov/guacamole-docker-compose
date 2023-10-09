# guacamole-docker-compose

docker-compose file for Apache Guacamole

### Pre-requisites

You need to create some directories where you checkout the docker-compose.

```bash
mkdir init
chmod -R +x ./init

mkdir data
mkdir record
mkdir drive
```

Now we need to run the init script for the database

```bash
sudo docker run --rm guacamole/guacamole /opt/guacamole/bin/initdb.sh --postgresql > ./init/initdb.sql
```

### Reset
To reset to the initial state, you need to delete the content of the folders you have created in the pre-requisites.
