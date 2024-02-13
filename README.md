# Monero-Wallet-Rpc

## DockerHub
https://hub.docker.com/r/chekist32/monero-wallet-rpc

## Example usage

```docker-compose.yml```
```yml
version: '3'

services:
  monero-rpc-test:
    image: chekist32/monero-wallet-rpc
    ports:
      - 38083:38083
    volumes:
      - /path_to_your_wallet_dir/:/monero/wallet
    command: 
      - "--stagenet" 
      - "--daemon-address=stagenet.community.rino.io:38081"
      - "--trusted-daemon"
      - "--rpc-bind-port=38083" 
      - "--rpc-login=user:pass" 
      - "--wallet-dir=/monero/wallet"

```
