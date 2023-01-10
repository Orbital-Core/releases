This repo contains Orbital builds for download. You can find the builds in the releases of this repo.

## Steps to run a single node:

```
docker pull couchdb
docker run -p 5984:5984 -d -e COUCHDB_USER=admin -e COUCHDB_PASSWORD=password couchdb

git clone https://github.com/Orbital-Core/orbital

cd orbital

cp -r tendermint_config_example tendermint_config

go build
./orbital
```
