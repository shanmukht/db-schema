# Setup Instructions

## DB installation

1. Make sure postgres is installed and able to login with postgres/postgres credentials.
2. Need to create user/role before we run the script.
	** Create Role:**
```sh
    CREATE ROLE kloopzcm WITH LOGIN PASSWORD 'kloopzcm'
```
   ###### Create User: 
```sh
	CREATE USER kloopzcm WITH PASSWORD 'kloopzcm';
``` 
3. Execute DDL/DML

Make sure db-schema/db/install-db.sh contains valid PSQL variable as follows or relevant.
```sh
    export PSQL=/usr/local/Cellar/postgresql/9.5.4/bin/psql
    $ cd db-schema/db
    $ ./install-db.sh
```

* make sure no clients are connected, stop tomcat first


## Meta model load

See the packer repository README.md
