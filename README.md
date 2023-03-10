This repo contains Orbital builds for download. You can find the builds in the releases of this repo.

## Steps to run a single node:

First you need to run the CouchDB database which is required by orbital node:

```
docker pull couchdb
docker run -p 5984:5984 -d -e COUCHDB_USER=admin -e COUCHDB_PASSWORD=password couchdb
```

Then download the latest release from [here](https://github.com/Orbital-Core/releases/releases) based on your OS or using this command, for example, in a CLI:

```
wget https://github.com/Orbital-Core/releases/releases/download/v1.1.0/Linux.zip
```

Unzip the folder and then `cd` inside the directory. 

After that run the below command to configure the node:

```
cp -r tendermint_config_example tendermint_config
```

Finally run the node using the below command

```
./orbital
```
