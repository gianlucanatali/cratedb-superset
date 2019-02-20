# Superset

This project is a fork of: https://github.com/amancevice/superset please have a look at that repo for additional info and docs.

The scope of this project is to test crateDB in conjunction with Apache superset.

## Prerequisites

The docker compose reference a docker image, you need to build it in your system from here:
https://github.com/gianlucanatali/docker-crate

Download the github project and build it using the command:

```docker build -t gianluca/crate:nightly .```

## Test CrateDB docker

Navigate to the [`examples/cratedb`](./examples/cratedb) directory  and run 

```docker-compose up```


## Database Initialization

After starting the Superset server, initialize the database with an admin user and Superset tables using the `superset-init` helper script:

If running a sample like postgres run this instead:
```bash
docker exec -it cratedb_superset_1 superset-demo
```
