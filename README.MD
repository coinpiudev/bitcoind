# Bitcoin Core Docker Image

## Docker Hub

This repository is fork from [XJonathanLEI/bitoind-docker](https://github.com/xJonathanLEI/bitcoind-docker).

Built images are available at [Docker Hub](https://hub.docker.com/r/coinpiu/bitcoind).

## Build

```bash
docker build --build-arg BITCOIN_CORE_VERSION=xxx -t coinpiu/bitcoind:xxx .
```

## Data Storage

`bitcoind` stores data in `/data`

## Environment Variables

### CHAIN

The network for `bitcoind` to run on. Can be one of the following:

- main
- test
- regtest

Defaults to `main`

### TXINDEX

Whether to maintain a full transaction index or not. Can be one of the following:

- true
- false

Defaults to `false`

### RPC_USERNAME

Username for RPC, defaults to `bitcoin`

### RPC_PASSWORD

Password for RPC, defaults to `bitcoin`
